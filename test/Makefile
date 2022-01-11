TOPDIR=..

include $(TOPDIR)/rule.mk

BINS=bilinearspeedtest rsaspeedtest generate_random suffixtest flinttest proposed_algorithm testAccUp testMerkle testproposed testboneh testminichain testMMRTree testTXOproof testbonehTXO testcctxo testmctxo update_witness_boneh testWitUp updatetxproof#libtest libtest1 libdirecttest
CFLAGS+=$(DCLXVI_INC) $(CRYPTOPP_INC)
LIBS=$(ACCUMLIB_FLG) $(DCLXVI_LIB_FLG) $(CRYPTOPP_LIB_FLG) $(GMP_LIB_FLG) -lflint -lmpfr
all:	$(BINS)

generate_random: generate_random.o
	$(CPP) $(CFLAGS) -o generate_random generate_random.o $(LIBS)

flinttest: flinttest.o
	$(CPP) $(CFLAGS) -o flinttest flinttest.o $(LIBS)

bilinearspeedtest: bilinearspeedtest.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o bilinearspeedtest bilinearspeedtest.o $(LIBS)

rsaspeedtest: rsaspeedtest.o $(ACCUMLIB)
	$(CPP) $(CFLAGS)  -o rsaspeedtest rsaspeedtest.o $(LIBS)

suffixtest: suffixtest.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o suffixtest suffixtest.o $(LIBS)

libtest: libtest.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o libtest libtest.o $(LIBS)

libtest1: libtest1.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o libtest1 libtest1.o $(LIBS)

libdirecttest: libdirecttest.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o libdirecttest libdirecttest.o $(LIBS)

proposed_algorithm: proposed_algorithm.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o proposed_algorithm proposed_algorithm.o $(LIBS)

testAccUp: testAccUp.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testAccUp testAccUp.o $(LIBS)

testMerkle: testMerkle.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testMerkle testMerkle.o $(LIBS)

testproposed: testproposed.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testproposed testproposed.o $(LIBS)

testminichain: testminichain.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testminichain testminichain.o $(LIBS)

testboneh: testboneh.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testboneh testboneh.o $(LIBS)
	
testMMRTree: testMMRTree.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testMMRTree testMMRTree.o $(LIBS)

testTXOproof: testTXOproof.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testTXOproof testTXOproof.o $(LIBS)

testbonehTXO: testbonehTXO.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testbonehTXO testbonehTXO.o $(LIBS)

testcctxo: testcctxo.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testcctxo testcctxo.o $(LIBS)

testmctxo: testmctxo.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testmctxo testmctxo.o $(LIBS)

update_witness_boneh: update_witness_boneh.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o update_witness_boneh update_witness_boneh.o $(LIBS)
	
testWitUp: testWitUp.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o testWitUp testWitUp.o $(LIBS)

updatetxproof: updatetxproof.o $(ACCUMLIB)
	$(CPP) $(CFLAGS) -o updatetxproof updatetxproof.o $(LIBS)
clean:
	rm -f *.o $(BINS)
