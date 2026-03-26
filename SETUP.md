# Setup

Step 1: Clone the repo and cd into the folder.

Step 2: Run this to install our output-cleaner:

```bash
python -m pip install nbstripout
```

Step 3: Run this to attach it to the repo:

```bash
python -m nbstripout --install
```

## The Final Push (Including Outputs)

Weeks from now, when the project is 100% finished and you are ready to submit, you need to turn off the filter so your graders can see the plots.

### Uninstall the filter

```bash
nbstripout --uninstall
```

### Generate the final results

Open your notebooks, click **Kernel > Restart & Run All**, and save them so the outputs are perfectly generated.

### Commit and push one last time

```bash
git add .
git commit -m "Final submission: included all cell outputs for grading"
git push
```

This workflow guarantees you won't bloat your repository during development, but ensures the grader gets exactly what they need at the end.
