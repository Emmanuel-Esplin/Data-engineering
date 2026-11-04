# PySpark Ingestion Practice

A personal practice notebook for reading and cleaning data with PySpark. It follows the Chapter 1 recipes in Packt's [Data Engineering with Databricks Cookbook](https://github.com/PacktPublishing/Data-Engineering-with-Databricks-Cookbook), and many cells are adapted from them.

This is exploratory learning work, not a pipeline. For a complete project, see [nyc-taxi-pipeline](https://github.com/Emmanuel-Esplin/nyc-taxi-pipeline).

## What the notebook covers

`Project 1.ipynb` runs Spark locally (`local[*]`) and works through:

| Topic | Techniques |
| --- | --- |
| CSV | Inferred and explicit schemas, null values and date formats |
| JSON | Multiline files, schema enforcement, corrupt-record handling, `get_json_object` and `json_tuple` |
| Nested data | `explode`, `explode_outer`, `array_distinct` and `array_contains` |
| Text | Cleaning review text with `regexp_replace` |

## Running it

The datasets are not in this repository. Download them from the [cookbook's `data` folder](https://github.com/PacktPublishing/Data-Engineering-with-Databricks-Cookbook/tree/main/data) into a local `data/` folder:

- `netflix_titles.csv`
- `nobel_prizes.json`
- `Stanford Question Answering Dataset.json`
- `Reviews.csv`

Then install PySpark and Jupyter, which need a compatible JDK:

```bash
pip install pyspark jupyterlab
jupyter lab
```

The notebook has not been cleaned up into a reproducible project, so some cells may need adjusting.

## License

MIT, see [LICENSE](LICENSE). Packt's copyright notice is kept because the notebook adapts its MIT-licensed cookbook code.
