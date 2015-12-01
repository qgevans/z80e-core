OBJECTS=cpu.o registers.o

../libz80e-core.a: ${OBJECTS}
	ar -rcs ../libz80e-core.a ${OBJECTS}

clean:
	-rm ${OBJECTS}
	-rm ../libz80e-core.a

.SUFFIXES: .o
.c.o:
	cc -I ../include -o ${.TARGET} -c ${.IMPSRC}
