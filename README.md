# nx-microfe-sample


## How this repo was set up
- Create workspace `npx create-nx-workspace@latest <workspace_name>`
- Remove default app `npx nx g rm <workspace_name>`
- Create shell app and two remotes 
    - `npx nx g @nx/react:host apps/shell --remotes=shop,cart` 
- Create a new remote app
    - `npx nx g @nx/react:remote apps/about --host=shell`
- Create lib folder for shared logic 
    - `npx nx g @nx/react:lib libs`
    - connect lib to shell and remotes
- Run it
    - `npx nx serve shell --devRemotes=cart,shop,about`


## Useful links

Learn more:

- [Learn more about this workspace setup](https://nx.dev/getting-started/tutorials/react-monorepo-tutorial?utm_source=nx_project&amp;utm_medium=readme&amp;utm_campaign=nx_projects)
- [Learn about Nx on CI](https://nx.dev/ci/intro/ci-with-nx?utm_source=nx_project&utm_medium=readme&utm_campaign=nx_projects)
- [Releasing Packages with Nx release](https://nx.dev/features/manage-releases?utm_source=nx_project&utm_medium=readme&utm_campaign=nx_projects)
- [What are Nx plugins?](https://nx.dev/concepts/nx-plugins?utm_source=nx_project&utm_medium=readme&utm_campaign=nx_projects)

