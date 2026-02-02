
## 📋 How to use as a Template

1.  **Duplicate the folder**:
    ```bash
    cp -r template my-new-project
    cd my-new-project
    ```

2.  **Initialize**:
    ```bash
    npm install
    ```

3.  **Rename Project**:
    - Update `name` in `package.json`.
    - Update `saas.config.ts`.
    - Create `.env.local` from example.

4.  **Updates**:
    - If you want to update the master template, go back to the `template` folder, make changes, run `npm run cleanup`, and commit.

## 🤖 AI Startup Prompts

Use these prompts to kickstart your project with **Antigravity** (Gemini):

### 1. New Project Kickoff
> "I have cloned the **SaaS Template**.
> My new project is called **[Project Name]**.
> Description: **[Short description of your idea]**.
> 
> Please:
> 1. Analyze the `saas.config.ts` and propose changes for this idea.
> 2. Create a `task.md` with a plan to transform this template into the MVP.
> 3. Suggest the necessary Supabase tables."

### 2. Add Feature
> "I need to add **[Feature Name, e.g., Blog]** to this project.
> We are using Next.js 15, Tailwind v4, and shadcn/ui.
> 
> 1. Check if `saas.config.ts` needs a feature flag.
> 2. Create the necessary files in `src/app`.
> 3. Update the navigation in config."

### 3. UI/UX Polish
> "Review the current page **[URL or Path]**.
> Apply the **'SaaS Template'** aesthetic:
> - Make it look premium and expensive.
> - Add micro-animations (framer-motion).
> - Clean up the spacing and typography."
