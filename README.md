### Minimal Makefile ā”
_Automatic Makefile for C and C++_
```
# build shared library with -fPIC, -shared
CFLAGS   = -g # -O3 # -fPIC  # CXXFLAGS for .cpp
LDFLAGS  = # -L../hello # -shared
LDLIBS   = # -lhello
CPPFLAGS = -MMD -MP # -I../hello
#CC      = $(CXX)  # link with CXX for .cpp

# target name is basename of one of the source files
main : $(patsubst %.c,%.o,$(wildcard *.c))  # .cpp
-include *.d
clean : ; -rm -fr *.o *.d
.PHONY : clean
```

<!--
**ljhm/ljhm** is a āØ _special_ āØ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- š­ Iām currently working on ...
- š± Iām currently learning ...
- šÆ Iām looking to collaborate on ...
- š¤ Iām looking for help with ...
- š¬ Ask me about ...
- š« How to reach me: ...
- š Pronouns: ...
- ā” Fun fact: ...
-->
