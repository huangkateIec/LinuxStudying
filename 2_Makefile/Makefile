CXX = g++
SRC_PATH =./src
INC_PATH = ./include
SRC = $(wildcard *.c) $(wildcard *.cpp)
#OBJ = $(patsubst %.c %.cpp, %.o, $(SRC))
OBJ = main.o hw_api.o
EXE = myapp

all: buildDir buildObj output

buildDir: 
	mkdir -p $(SRC_PATH)  $(INC_PATH) 

buildObj: $(SRC)
	$(CXX) -c $(SRC)

output: $(OBJ)
	@echo $(OBJ)
	$(CXX) -o $(EXE) $(OBJ)

clean:
	rm -rf $(OBJ) $(EXE) $(SRC_PATH)  $(INC_PATH) 
