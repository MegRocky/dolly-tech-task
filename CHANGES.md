# Meg Rocky Dolly Tech Assesment - Changes

## Bugs / Errors

**Bug 1** - Incorrect HTTP method for updating - using POST instead of PUT

    updated noteService.ts to use PUT in update Note

**Bug 2** - Not preserving the createdAt date during updates

    removed assigning the createdAt date in the storage.ts update function given that the created at date will be present in the spread updateNoteDto

**Bug 3** - deleting without confirming

    updated noteItem.tsx to provide a confirmation window and set the is deleting state to false if the window rejects

**Bug 4** - syntax error in noteService.ts

    Closed bracket in noteService.ts

**Bug 5** - updates/new notes not working, note form wasn't using the onSubmit function passed from the page.

    NoteForm.tsx - added calling the onSubmit function in handleSubmit with the data variable

## Dark Mode

Implemented the toggle button as a client component so it would work with the event listener. I placed it in the footer so it will effect all components. The toggle functionality makes use of use effect hook and local storage to access users previous theme choice.

## Acessibility

Missing form label from search bar:

    added ARIA Label

Low colour contrast on navigation links and create new note button:

    edited colours in both dark and light mode

## Other

Tidied up console logs
