## Workspace
A skeleton app is provided to get you started in the app directory.

After checkout, run this to install dependencies:

    cd app
    npm install

You may find it easier to use Docker to manage the node environment. To
do the initial module install:

    docker run --rm -it \
               -v $(pwd)/app:/app -u `id -u`:`id -g` \
               -w /app node:23-bookworm \
               npm install

To run the app:

    docker run --rm -it \
               -v $(pwd)/app:/app -u `id -u`:`id -g` \
               -w /app -p 5173:5173 \
               node:23-bookworm \
               npm run dev

## Create a simple to-do list application.
- Implement an input field and an add button that appends new tasks to a task list.
- Display the list of tasks below the input field.
- Include a checkbox or a button to mark each task as completed.
- Style it to show a clear distinction between completed and pending tasks.
- If time permits, add a delete button to remove tasks.

## Guidelines
- Use functional components with hooks (useState, useEffect).
- Do not rely on external state management libraries (redux, mobx, etc.).
- Demonstrate a clear understanding of basic react concepts such as state, props, and rendering lists.
- This should take 30 to 45 minutes

