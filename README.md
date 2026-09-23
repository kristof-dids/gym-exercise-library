# Gym Exercise Library

A personal, self-contained exercise reference for gym-floor use: pick a muscle group, see the exercises that hit it, and get a one-line form cue for each one.

- 217 exercises across 10 muscle groups (Chest, Back, Shoulders, Biceps, Triceps, Abs & Core, Legs, Glutes, Calves, Forearms)
- Mix of bodyweight, dumbbell, barbell, machine and cable movements
- Primary + secondary muscles shown per exercise, plus a brief cue on correct form
- Responsive light interface with large studio-style instructional images, orange movement cues and highlighted target muscles
- Equipment filter and cross-group search
- Static `index.html` + exercise data, no build step or dependencies

## Usage

Open `index.html` directly in a browser, or serve the folder with any static file server.

## Image credits

Legacy demonstration photos in `images/` are sourced from [free-exercise-db](https://github.com/yuhonas/free-exercise-db), released under the [Unlicense](https://github.com/yuhonas/free-exercise-db/blob/main/LICENSE) (public domain). They remain available only as automatic fallbacks.

The redesigned assets in `images/studio/` were generated specifically for this project with OpenAI's image-generation tool. Their consistent art direction and prompt template are documented in `IMAGE_STYLE.md`.

## Hosting on GitHub Pages

Settings → Pages → Deploy from branch → `main` / `(root)`. The site will then be available at:

`https://kristof-dids.github.io/gym-exercise-library/`
