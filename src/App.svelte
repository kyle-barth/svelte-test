<style>
  @import "./App.svelte.css";
</style>

<script lang="typescript">
  import Sidebar from "./components/sidebar/Sidebar.svelte";
  import ViewNote from "./components/ViewNote/ViewNote.svelte";

  import type { Note } from "types/models/Note";
  import type { UpdateNote } from "types/models/UpdateNote";

  let note: Note | undefined = undefined;

  const updateNote: UpdateNote = (previewNote: Note) => (note = previewNote);
</script>

<div class="container">
  <Sidebar {updateNote} />

  {#if note}
    <ViewNote {note} />
  {/if}
</div>
