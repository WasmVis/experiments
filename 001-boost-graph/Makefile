all: file-dependency-example kevin-bacon

INC=-I/usr/local/include

# DEBUGFLAGS=-g -s DEMANGLE_SUPPORT=1

CXXFLAGS=-std=c++11 -s WASM=1 -O3 -Os $(DEBUGFLAGS)

file-dependency-example:
	$(CXX) $(CXXFLAGS) $(INC) file-dependency-example.cpp -o build/file-dependency-example.html

kevin-bacon:
	$(CXX) $(CXXFLAGS) $(INC) kevin-bacon.cpp -o build/kevin-bacon.html --embed-file kevin-bacon.dat
clean:
	rm -rf build/*
