Added filtering to the todo app so you can switch between All, Active, and Done todos.
Backend: getTodos now checks for a `done` query param and filters based on that. No param = everything, same as before.
Frontend: fetchTodos can take a filter now and sends it in the request. Added a filter state in App.jsx and three buttons (All/Active/Done) that update it, which re-fetches the todos whenever you click one.
Went with server-side filtering (new request every click) instead of filtering what's already loaded, since the task wanted us to practice passing query params.
