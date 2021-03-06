# shabam
A python tool to create sequence plots from bam/cram files.

The dream:

```
import shabam
shabam.plot('sequence.bam', chrom=2, start=48000000, end=48000080, file='plot.png')
```

![The dream](/dream.png?raw=true)

## The steps

#### Create text based view (similar to samtools tview)
- [ ] Extract reads from a file
- [ ] Read a reference file
- [ ] Line up reads from a bam with a reference
- [ ] Print reads in terminal
- [ ] Optimize vertical height

#### Sequence plot
- [ ] Plot a list of letters using [matplotlib patches](http://matplotlib.org/api/patches_api.html)
- [ ] Scale colors based on qual values
- [ ] Save plot

#### Historgram plot
- [ ] Compute proportion of variants at any site
- [ ] Plot read depth
- [ ] At positions with proportion of variants > threshold, reflect proportion with base colors

## Development setup
1. Install python 2 ([try miniconda](http://conda.pydata.org/miniconda.html) if you haven't got it)
2. Install [pysam](https://github.com/pysam-developers/pysam/)
3. Ensure git is installed (try `git --version`)
4. Ensure you have a github account.
5. Fork this repository and clone onto your local machine.

## References
- [genome.sph.umich.edu/wiki/SAM](http://genome.sph.umich.edu/wiki/SAM)

