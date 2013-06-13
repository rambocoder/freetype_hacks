freetype-hacks
==============

libfreetype patches to have awesome looking Linux fonts

Clone the latest libfreetype

```
git clone http://git.sv.nongnu.org/r/freetype/freetype2.git
cd freetype2
patch -p1 < ../configurable-branch
./autogen.sh
chmod u+x run.sh
./run.sh
```

Set environment variables

```
export CHROMEOS_SHARPENING_STRENGTH=10
export CHROMEOS_GAMMA_STRENGTH=150

export FT_FILTER_PARAMS="16 64 112 64 16"
```