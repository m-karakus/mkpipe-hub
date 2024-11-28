# mkpipe-hub

`mkpipe-hub` is the central registry for all official and community-contributed plugins for the `mkpipe` ecosystem.  
Here, you can discover extractors, loaders, and utilities to extend your `mkpipe` workflows.

---

## Plugin Registry

The main plugin registry is maintained in [plugins.yaml](plugins.yaml).  
This includes details about all available plugins and their metadata, including repositories, PyPI links, and descriptions.

---

### How to Contribute

If you’ve built an extractor or loader for `mkpipe`, feel free to add it to the registry by following these steps:
1. Fork this repository.
2. Add your plugin to `plugins.yaml` using the format below:
   ```yaml
   extractors:
     - name: "PostgreSQL Extractor"
       repo: "https://github.com/m-karakus/mkpipe-extractor-postgres"
       pypi: "https://pypi.org/project/mkpipe-extractor-postgres/"
       author: "m-karakus"
       description: "Extract data from PostgreSQL databases."

   loaders:
     - name: "S3 Loader"
       repo: "https://github.com/m-karakus/mkpipe-loader-s3"
       pypi: "https://pypi.org/project/mkpipe-loader-s3/"
       author: "m-karakus"
       description: "Load data into Amazon S3."
   ```

3. (Optional) Add a `.md` file to the appropriate folder (`extractors/` or `loaders/`) with detailed documentation.
4. Submit a pull request!

---

### Explore Plugins

#### Extractors
- [PostgreSQL Extractor](extractors/postgres.md)
- [MySQL Extractor](extractors/mysql.md)

#### Loaders
- [S3 Loader](loaders/s3.md)
- [BigQuery Loader](loaders/bigquery.md)

---

### Community Plugins
Check out the [Awesome Community Plugins](community/awesome-community-plugins.md) list for unofficial contributions from the `mkpipe` community.

---

### Support Me
<iframe src="https://github.com/sponsors/m-karakus/button" title="Sponsor m-karakus" height="32" width="114" style="border: 0; border-radius: 6px;"></iframe>