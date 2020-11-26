<style>
  @import "./ViewNote.svelte.css";
</style>

<script lang="typescript">
  import type { Note } from "types/models/Note";

  export let note: Note;
</script>

<div class="note">
  <div class="note-container">
    <div style="display: inline-flex">
      <p class="title">{note.id}) {note.title}</p>
    </div>
    <p class="note-body">{note.body}</p>
  </div>
</div>
