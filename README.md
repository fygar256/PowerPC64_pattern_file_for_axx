# Pattern file of PowerPC64 for axx

ppc64isa.axx common file for ppc64le.axx and ppc64.axx

ppc64le.axx  pattern file for powerpc64 little endian

ppc64.axx    pattern file for powerpc64 big endian

ppc64_test.s test assembly file

### to test:

```
caxx ppc64.axx ppc64_hello.s -o ppc64_hello.o
ld.lld ppc64_hello.o -o ppc64_hello
qemu-ppc64-static ./ppc64_hello              

caxx ppc64.axx bf_ppc64.s -o bf_ppc64.o
ld.lld bf_ppc64.o -o bf_ppc64
qemu-ppc64-static ./bf_ppc64 ../mandelbrot.bf```
