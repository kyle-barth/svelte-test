<style>
  @import "./PreviewNote.svelte.css";
</style>

<script lang="typescript">
  import type { Note } from "types/models/Note";
  import type { SelectNote } from "types/models/SelectNote";

  export let notes: Note[];
  export let selectNote: SelectNote;

  const handleClick: (id: number) => Note = (id: number) => selectNote(id);
</script>

{#each notes as note}
  <div on:click={(e) => handleClick(note.id)} class="preview-note">
    <div class="note-container">
      <p class="title">{note.title}</p>
      <p class="body">{note.body}</p>
    </div>
  </div>
{/each}
