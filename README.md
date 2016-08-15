![dag](resources/dag.png)

# Install

+ snakemake
+ biom-format
+ usearch
+ clustalo
+ fasttree


# Usage

Place demultiplexed, uncompressed reads into `results/<EXPERIMENT NAME>/demux`
with a `.fastq` file extension.

To run the workflow across 24 cores:

```
snakemake -j 24 --configfile resources/16s.config.yaml --config eid=<EXPERIMENT NAME>
```

Results are written to `results/<EXPERIMENT NAME>/<PERCENT ID>/`.

Methods and summary data can be found in `results/<id>/<percent_identity>/README.html`

![readme](resources/readme_example.png)
