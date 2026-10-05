# Feature Engineering

Feature engineering is the preprocessing step that turns raw data into features that better represent the underlying problem for a predictive model, often by applying domain knowledge. This repository covers the core techniques and the scikit-learn tools that put them into a clean, reproducible workflow. Before starting the notebooks, read the [machine learning workflow notes](machine_learning_workflow.md).

## Learning Objectives

By the end of this repository, you should be able to:

- Handle missing values with imputation.
- Encode categorical variables and scale numeric features.
- Expand and discretize features to capture more signal.
- Combine preprocessing steps with `ColumnTransformer` and `Pipeline` for a reproducible workflow.

## Learning Path

Work through the notebooks in order. The `1.x` notebooks cover the basics, the `2.x` notebooks cover advanced workflow tools, and each lesson is followed by an exercise:

| File / Folder | Description |
|---|---|
| [**1.1 - Intro to Feature Engineering**](1.1_intro_to_fe.ipynb) | Imputation, categorical encoding, feature scaling, and feature expansion. |
| [**1.2 - Intro Exercise**](1.2_intro_to_fe_exercise.ipynb) | Practice transforming raw data into a form suitable for modeling. |
| [**2.1 - Advanced Feature Engineering**](2.1_advanced_fe.ipynb) | Building reproducible workflows with `ColumnTransformer` and `Pipeline`. |
| [**2.2 - Advanced Exercise**](2.2_advanced_fe_exercise.ipynb) | Apply `ColumnTransformer` and `Pipeline` to a new transformation task. |

### Additional Folders and Files

| File / Folder | Description |
|---|---|
| [**Machine Learning Workflow**](machine_learning_workflow.md) | Background reading on where feature engineering fits in the ML workflow. |
| [**Data**](data/) | Datasets used across the notebooks. |
| [**Assets**](assets/) | Images used in the notebooks and cheatsheet. |
| [**Visual Reference**](assets/cheatsheet_feature_engineering.html) | Optional browser-based summary with saved illustrations. Run the notebooks for current results. |
| [**Solutions**](solutions/) | Reference solutions. |
| [**pyproject.toml**](pyproject.toml) | Project configuration and dependencies. |
| [**uv.lock**](uv.lock) | Dependency lock file. |

## Setup

> [!NOTE]
> Throughout these steps, text in angle brackets like `<repo-name>` is a
> **placeholder**. Replace it, including the `< >` brackets, with your own
> value. For example, `cd <repo-name>` becomes `cd ds-feature-engineering`.

### 1. Create the Repository from the Template

Click **Use this template** on GitHub.

When creating the repository:

- Set yourself as the **Owner**
- Choose a repository name
- Disable **Include all branches**
- Click **Create repository**

> [!IMPORTANT]
> If you are working in pairs or groups, only **one person** should complete this step.

---

### 2. Add Collaborators (Pairs/Groups Only)

If working with teammates:

1. Open the repository on GitHub
2. Go to **Settings → Collaborators**
3. Add your teammates as collaborators
4. Share the repository link with your team

Teammates should accept the invitation before continuing.

---

### 3. Clone the Repository

Copy the SSH URL from the **Code** button on GitHub, then run:

```bash
git clone <copied-ssh-url>
```

The copied SSH URL will look like `git@github.com:<your-username>/<repo-name>.git`.

---

### 4. Move into the Project Folder and Install Dependencies

This installs all dependencies and creates a virtual environment in `.venv/`.

```bash
cd <repo-name>
uv sync
```

---

### 5. Open the Notebooks

> [!NOTE]
> Make sure you open VS Code from the project root so it automatically detects the environment created by `uv sync`.

Launch VS Code in the project root folder:

```bash
code .
```

Then open a notebook and select the Python environment created by `uv sync` as the kernel.

## References & Further Reading

- [**Scikit-learn: Preprocessing data**](https://scikit-learn.org/stable/modules/preprocessing.html): Official reference for imputation, encoding, scaling, and discretization.
- [**Scikit-learn: Pipelines and composite estimators**](https://scikit-learn.org/stable/modules/compose.html): How `ColumnTransformer` and `Pipeline` fit together.
- [**Scikit-learn: Compare the effect of different scalers**](https://scikit-learn.org/stable/auto_examples/preprocessing/plot_all_scaling.html): A visual comparison of scaling methods on real data.
- [**Discover Feature Engineering**](https://machinelearningmastery.com/discover-feature-engineering-how-to-engineer-features-and-how-to-get-good-at-it/): A practical overview of feature engineering in applied projects.
