# bintel-02-mining

[![Workflow Guide](https://img.shields.io/badge/Pro--Guide-pro--analytics--02-green)](https://jrwebb7.github.io/pro-analytics-02/workflow-b-apply-example-project/)
[![Python 3.14](https://img.shields.io/badge/python-3.14%2B-blue?logo=python)](./pyproject.toml)
[![MIT](https://img.shields.io/badge/license-see%20LICENSE-yellow.svg)](./LICENSE)

> Professional Python project: mining and exploring smart sales data.

## Project Description

This project focuses on reading raw business data into pandas DataFrames
for exploration and analysis.

We work with a realistic smart sales dataset containing
customers, products, and sales records.

We learn to:

- read raw CSV files into reusable pandas DataFrames
- inspect distributions of customers, products, and sales
- identify data quality issues that will need cleaning
- visualize price distributions and sales trends over time
- add reusable inspection and quality-check functions to the BI pipeline

## Working Files

You'll work with these areas:

- **data/raw** - raw smart sales CSV files (customers, products, sales)
- **docs/** - project narrative and documentation
- **src/bizintel/** - the app is an example; run only (no need to modify)
- **pyproject.toml** - update authorship & links
- **zensical.toml** - update authorship & links

## Instructions (pro-analytics-02)

Follow the
[step-by-step workflow guide](https://jrwebb7.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to complete:

1. Phase 1. **Start & Run**
2. Phase 2. **Change Authorship**
3. Phase 3. **Read & Understand**
4. Phase 4. **Modify**
5. Phase 5. **Apply**

## Challenges

Challenges are expected.
Sometimes instructions may not quite match your operating system.
When issues occur, share screenshots, error messages, and details about what you tried.
Working through issues is part of implementing professional projects.

## Success

After completing Phase 1. **Start & Run**,
you'll have your own GitHub project,
and running the example module will print out:

```shell
========================
Executed successfully!
========================
```

A new file `project.log` will appear in the root project folder.

## Command Reference

<details>
<summary>Show command reference</summary>

## Custom Project Commands

Run the Phase 4 customized mining analysis:

```shell
uv run python -m bizintel.mining_case_james
```

### In a machine terminal (open in your `Repos` folder)

After you get a copy of this repo in your own GitHub account,
open a machine terminal in your `Repos` folder:

```shell
# Replace username with YOUR GitHub username.
git clone https://github.com/username/bintel-02-mining
```

cd bintel-02-mining
code .
```

### In a VS Code terminal

These are listed for convenience.
For best results, follow the detailed instructions in
[pro-analytics-02 guide](https://jrwebb7.github.io/pro-analytics-02/).

```shell
uv self update
uv python pin 3.14
uv lock --upgrade
uv sync --extra dev --extra docs --upgrade

uvx pre-commit install
uvx pre-commit autoupdate

git add -A
uvx pre-commit run --all-files
# repeat if changes were made
uvx pre-commit run --all-files

# run the example module
uv run python -m bizintel.mining_case

# run common chores
uv run ruff format .
uv run ruff check . --fix
uv run python -m pyright
uv run python -m pytest
uv run python -m zensical build

# save progress
git add -A
git commit -m "update"
git push -u origin main
```

</details>

## Notes

- Use the **UP ARROW** and **DOWN ARROW** in the terminal to scroll through past commands.
- Use `CTRL+f` to find (and replace) text within a file.
- You do not need to add to or modify `tests/`. They are provided for example only.
- Many files are silent helpers. Explore as you like, but nothing is required.
- You do NOT need to understand everything; understanding builds naturally over time.

## Troubleshooting >>>

If you see something like this in your terminal: `>>>` or `...`
You accidentally started Python interactive mode.
It happens.
Press `Ctrl+c` (both keys together) or `Ctrl+Z` then `Enter` on Windows.

## Example Output (Remove this Section after You Verify)

```shell
| INFO | ML | ========================
| INFO | ML | Executed successfully!
| INFO | ML | ========================
```

## Findings and Visuals

Take screenshots of your charts and provide them here with a discussion.
In Markdown, display a figure using:
an exclamation mark immediately followed by square brackets containing a useful caption
immediately followed by parentheses containing the relative path to your figure.

In your custom project:

- your figures and narrative should reflect your work
- this `README.md` should include your commands, process, and visuals
- `docs/index.md` should include your narrative

Replace these placeholders with screenshots from your own project run:

![Total Sales by Region](./docs/images/Figure_1.png)

![Total Sales by Product Category](./docs/images/Figure_2.png)

## Project Documentation

Additional project instructions, terms, and notes:

[docs/index.md](docs/index.md)

## Phase 4: Make a Technical Modification

For Phase 4, I created a customized copy of the working mining example named `mining_case_james.py`. I modified the product price distribution histogram by increasing the number of bins from 10 to 15. I also updated the chart title to identify the 15-bin visualization.

The purpose of this modification was to create a more detailed visualization of the distribution of product prices. Increasing the number of bins divides the range of product prices into smaller intervals, which provides a more granular view of the data.

I ran the customized project using the following command:

`uv run python -m bizintel.mining_case_james`

The project executed successfully and produced the modified product price distribution chart along with the existing sales trend analysis.

## Phase 5: Apply the Skills to a New Problem

For Phase 5, I applied the BI mining and exploration skills from the example project to analyze sales performance from two different business perspectives.

The custom analysis examines:

1. Total sales by customer region.
2. Total sales by product category.

The regional analysis combines customer and sales data to show how total sales differ across geographic regions. This can help identify stronger and weaker markets.

The product category analysis combines product and sales data to compare total sales across product categories. This can help identify which categories contribute the most to overall sales.

I ran the custom analysis using the following command:

`uv run python -m bizintel.app_case`

The project executed successfully and generated bar charts for total sales by region and total sales by product category. These visualizations provide unique results that can support business decisions related to regional performance and product strategy.

## Citation

[CITATION.cff](./CITATION.cff)

## License

[MIT](./LICENSE)
