BTOUCH=/Developer/MonoTouch/usr/bin/btouch

all: Parse.dll

Parse.dll: Makefile AssemblyInfo.cs ParseLib.cs Parse enums.cs
	$(BTOUCH) -unsafe ParseLib.cs AssemblyInfo.cs enums.cs --out=$@ --link-with=Parse,Parse --outdir=tmp

clean:
	-rm -f *.a *.dll
