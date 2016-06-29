<!-- AddToAny BEGIN -->
<div class="a2a_kit a2a_kit_size_32 a2a_default_style">
<a class="a2a_dd" href="//www.addtoany.com/share"></a>
<a class="a2a_button_facebook"></a>
<a class="a2a_button_twitter"></a>
<a class="a2a_button_google_plus"></a>
</div>
<script async src="//static.addtoany.com/menu/page.js"></script>
<!-- AddToAny END -->


This package implements methods to analyze and visualize functional profiles of genomic coordinates (supported by ChIPseeker), gene and gene clusters.

## Project website


`clusterProfiler` is released within the [Bioconductor](https://bioconductor.org/packages/clusterProfiler) project and the source code is hosted in <a href="https://github.com/GuangchuangYu/clusterProfiler"><i class="fa fa-github fa-lg"></i> GitHub</a>.

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.6.1/css/font-awesome.min.css">

Join the group chat in <a href="https://twitter.com/hashtag/clusterProfiler"><i class="fa fa-twitter fa-lg"></i></a> and <a href="http://huati.weibo.com/k/clusterProfiler"><i class="fa fa-weibo fa-lg"></i></a>.

## Citation

Please cite the following article when using `clusterProfiler`:

```
Yu G, Wang L, Han Y and He Q. 
clusterProfiler: an R package for comparing biological themes among gene clusters.
OMICS: A Journal of Integrative Biology, 2012, 16(5):284-287. 
```

## Installation

Install `clusterProfiler` is easy, follow the guide in the [Bioconductor page](https://bioconductor.org/packages/clusterProfiler/):

```r
## try http:// if https:// URLs are not supported
source("https://bioconductor.org/biocLite.R")
## biocLite("BiocUpgrade") ## you may need this
biocLite("clusterProfiler")
```

## Overview

It supports both *hypergeometric test* and *Gene Set Enrichment Analysis* for many ontologies/pathways, including:

+ Disease Ontology (via [DOSE](https://www.bioconductor.org/packages/DOSE))
+ [Network of Cancer Gene](http://ncg.kcl.ac.uk/) (via [DOSE](https://www.bioconductor.org/packages/DOSE))
+ Gene Ontology (supports many species with GO annotation query online via [AnnotationHub](https://bioconductor.org/packages/AnnotationHub/))
+ KEGG Pathway and Module with latest online data (supports more than 4000 species listed in <http://www.genome.jp/kegg/catalog/org_list.html>)
+ Reactome Pathway (via [ReactomePA](https://www.bioconductor.org/packages/ReactomePA))
+ DAVID (via [RDAVIDWebService](https://www.bioconductor.org/packages/RDAVIDWebService))
+ [Molecular Signatures Database](http://software.broadinstitute.org/gsea/msigdb)
	* hallmark gene sets
	* positional gene sets
	* curated gene sets
	* motif gene sets
	* computational gene sets
	* GO gene sets
	* oncogenic signatures
	* immunologic signatures
+ Other Annotations
	* from other sources (e.g. [DisGeNET](http://www.disgenet.org/web/DisGeNET/menu/home) as [an example](https://guangchuangyu.github.io/2015/05/use-clusterprofiler-as-an-universal-enrichment-analysis-tool/))
	* user's annotation
	* customized ontology
	* and many others
  
*clusterProfiler* also provides several visualization methods to help interpreting enriched results, including:

+ barplot
+ cnetplot
+ dotplot
+ enrichMap
+ gseaplot
+ plotGOgraph (via [topGO](https://www.bioconductor.org/packages/topGO) package)
+ upsetplot
  
and several useful utilities:

+ bitr (Biological Id TranslatoR)
+ compareCluster (biological theme comparison)
+ dropGO (screen out GO term of specific level or specific term)
+ go2ont (convert GO ID to Ontology)
+ go2term (convert GO ID to descriptive term)
+ gofilter (restrict result at specific GO level)
+ gsfilter (restrict result by gene set size)
+ simplify (remove redundant GO terms, supported via [GOSemSim](https://www.bioconductor.org/packages/GOSemSim))


## Documentation

### Vignettes

<https://bioconductor.org/packages/release/bioc/vignettes/clusterProfiler/inst/doc/clusterProfiler.html>

### Blog posts

<https://guangchuangyu.github.io/tags/clusterprofiler>



## Feedback ##

 - For bugs or feature request, please post to [github issue](https://github.com/GuangchuangYu/clusterProfiler/issues).
 - For user questions, please post to [google group](https://groups.google.com/forum/#!forum/clusterprofiler). We are also following every post tagged with **clusterProfiler** on [Bioconductor support site](https://support.bioconductor.org/) and [Biostars](https://www.biostars.org/).


## Comments

<div id="disqus_thread"></div>
<script type="text/javascript">

(function() {
    // Don't ever inject Disqus on localhost--it creates unwanted
    // discussions from 'localhost:1313' on your Disqus account...
    // if (window.location.hostname == "localhost")
    //     return;

    var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
    var disqus_shortname = 'gcyu';
    dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="http://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
<a href="http://disqus.com/" class="dsq-brlink">comments powered by <span class="logo-disqus">Disqus</span></a>

