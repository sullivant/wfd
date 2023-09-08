# Winsted Fire Department
Various documentation tracking for the Winsted Fire Department.  The main website can be located here: http://www.winstedfire.org

This is a personal project to keep track of some documentation that is already freely available on the website above.  Do not consider this the latest version unless we make the necessary workflow changes at the policy level.

## Documents
- `bylaws` : Original file located here: http://winstedfire.org/files.html ( See related file dates )


## Viewing Differences
When necessary a version on the official website can be compared to the version here by simply doing the normal software development 'thing' and letting git determine if there was a change.

When desired changes can be viewed in a diff file format but due to the binary files docx and pdf a third party library is required: `pandoc`.

### Comparing with Pandoc
Details on how to implement this on your local machine can be found here: https://github.com/vigente/gerardus/wiki/Integrate-git-diffs-with-word-docx-files  

This process does a good job at showing the deltas in a reportable and sensible fashion.  The two basic commands, after pandoc is installed and setup, are:

```bash
git log -p --word-diff=color bylaws/by-laws-09062023.docx 
```

```bash
git wdiff bylaws/by-laws-09062023.docx
```



