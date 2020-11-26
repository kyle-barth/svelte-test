<style>
  @import "./Sidebar.svelte.css";
</style>

<script lang="typescript">
  import PreviewNote from "./preview_note/PreviewNote.svelte";

  import type { UpdateNote } from "types/models/UpdateNote";
  import type { Note } from "types/models/Note";
  import type { SelectNote } from "types/models/SelectNote";

  export let updateNote: UpdateNote;

  let previewNotes: Note[] = [
    {
      id: 1,
      title: "test",
      body:
        "Veniam do magna pariatur excepteur eiusmod dolor. Incididunt sint magna dolor ut laborum ",
    },
    {
      id: 2,
      title: "test",
      body:
        "Veniam do magna pariatur excepteur eiusmod dolor. Incididunt sint magna dolor ut laborum ",
    },
    {
      id: 3,
      title: "test",
      body:
        "Veniam do magna pariatur excepteur eiusmod dolor. Incididunt sint magna dolor ut laborum ",
    },
  ];

  const selectNote: SelectNote = (id: number): Note => {
    const note: Note = previewNotes.find((x) => x.id === id) as Note;
    return updateNote(note);
  };
</script>

<div class="sidebar">
  <PreviewNote notes={previewNotes} {selectNote} />
</div>
