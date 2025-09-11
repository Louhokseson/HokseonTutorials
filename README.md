# HokseonTutorials

This work is authored by [Xuexun Lu (Hokseon Lou)](https://louhokseson.github.io).

> HokseonTutorials

is a collection of Julia scripts for tutorial purposes.

To (locally) reproduce this project, do the following:

0. Download this code base. Notice that raw data are typically not included in the
   git-history and may need to be downloaded independently.
1. Add Hokseon personal Julia registry in your local project enironment (if not done yet):
   ```
   (@v1.11) pkg> activate .
   (HokseonTutorials) pkg> registry add https://github.com/Louhokseson/HokseonRegistry.git
   ```
   for downloading some useful packages developed by Hokseon.
2. Open a Julia console and do:
   ```
   julia> using Pkg
   julia> Pkg.add("DrWatson") # install globally, for using `quickactivate`
   julia> Pkg.activate("path/to/this/project")
   julia> Pkg.instantiate()
   ```

This will install all necessary packages for you to be able to run the scripts and
everything should work out of the box, including correctly finding local paths.

You may notice that most scripts start with the commands:
```julia
using DrWatson
@quickactivate "HokseonTutorials"
```
which auto-activate the project and enable local path handling from DrWatson.
