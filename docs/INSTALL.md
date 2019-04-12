# Installation

The Sarek pipeline is already installed in legion and myriad. You just need to load nextflow and start using it:

```bash
module load blic-modules
module load nextflow

nextflow run /shared/ucl/depts/cancer/apps/nextflow_pipelines/Sarek/main.nf -profile --sample input_somatic.tsv --genome GRCh38 
```

You need to specify an appropiate configuration profile with the `-profile` argument. Please use the `legion` configuration profile [`conf/legion.config`](../conf/legion.config) if you submit it from 
legion, and the `myriad` config [`conf/myriad.config`](../conf/myriad.config) if you send the job from myriad.
