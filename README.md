## Why does Solid not persist state between HMRs?

To reproduce:

1. Go to any project. `cd <project>`

2. `bun install` then `bun dev` then open http://localhost:3000

3. Click on any "Counter", increase it (changes the state obviously).

4. Now make a change on the code of the project, and press save.

5. Expected Results:

- ✅ react-vite - state is persisted
- ✅ vue vite - state is persisted
- ❌ solid-start - state is NOT persisted
- ❌ solid-vike - state is NOT persisted
- ❌ solid-vite - state is NOT persisted
- ❌ svelte-vite - state is NOT persisted
- ❌ svelte-kit - state is NOT persisted
