bugs/errors

bug 1 Incorrect HTTP method for updating - using POST instead of PUT

updated noteService.ts to use PUT in update Note

bug 2 Not preserving the createdAt date during updates

bug 3 deleting without confirming

updated noteItem.tsx to provide a confirmation window and set the is deleting state to false if the window rejects

bug 4 - Closed bracket in noteService.ts

bug 5 - updates/new notes not happening as note form wasn't using the onSubmit function it was being passed from the page.

NoteForm.tsx - added calling the onSubmit function in handleSubmit with the data variable

dark mode

Implemented the toggle button as a client component so it would work with the event listener, the toggle makes use of use effect hook to access users previous theme choice.

other

Acessibility - missing form label from search bar
tidied up console.logs on main page
