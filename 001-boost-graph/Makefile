all: file-dependency-example kevin-bacon

INC=-I/usr/local/include

CXXFLAGS=-std=c++11 -s WASM=1 -g -s DEMANGLE_SUPPORT=1 -O3

file-dependency-example:
	$(CXX) $(CXXFLAGS) $(INC) file-dependency-example.cpp -o build/file-dependency-example.html

kevin-bacon:
	$(CXX) $(CXXFLAGS) $(INC) kevin-bacon.cpp -o build/kevin-bacon.html --preload-file kevin-bacon.dat
clean:
	rm -rf build/*
