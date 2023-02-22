objects = main.o addition.o division.o multiplication.o subtraction.o

calculator: $(objects) operations.h
	cc -o calculator $(objects)

$(objects): %.o:%.c operations.h
	cc -c $< -o $@

clean:
	rm -f calculator $(objects)

.PHONY: clean