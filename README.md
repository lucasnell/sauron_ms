
## Organization

This directory is organized with `__sauron.tex` as the main document.
It mostly sets up the document formatting and inputs the other files in the proper order.
The only actual content it contains is the keywords, title, and authors (although the 
latter is truncated for now due to AmNat's double-blind review process).

Most of the document text is in the `abstract.tex`, `introduction.tex`, `methods.tex`,
`results.tex`, `discussion.tex`, and `app_*.tex` files.
You should mostly be editing these files.

## Citations in the document:

> Thanks to Daijiang for these!

1. Go to [Google Scholar](https://scholar.google.com); click the top left, and select
  `Settings`; then in the `Bibliography manager` section, check 
  `show links to import citations into BibTeX`, then Save it. 
  This step only need to be done once.
2. Back to the Google Scholar homepage and search the paper you want to cite 
  (e.g., "Generalized linear mixed models for phylogenetic analyses of community structure"). Under the item, click the quotation marks, then click `BibTeX`.
  Then copy the whole new page (`Cmd + A` then `Cmd + C`).
  It should look something like this:

```
@article{ives2011generalized,
  title={Generalized linear mixed models for phylogenetic analyses of community structure},
  author={Ives, Anthony R and Helmus, Matthew R},
  journal={Ecological Monographs},
  volume={81},
  number={3},
  pages={511--525},
  year={2011},
  publisher={Wiley Online Library}
}
```

3. Open `refs.bib` in this folder, and paste the citation information there.
4. To cite the paper in the manuscript, copy its key (e.g. `ives2011generalized` here) 
  and insert it inside the proper LaTeX command (typically `\citep{ives2011generalized}`)
  to where you want to cite it. For multiple papers, use `\citep{key1, key2}`.
5. That's it.