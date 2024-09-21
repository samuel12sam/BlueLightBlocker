BUILD_FOLDER   := build
SOURCE_FILES   := $(wildcard *.c)
OBJECT_FILES   := $(patsubst %.c, $(BUILD_FOLDER)/%.o, $(SOURCE_FILES))
EXECUTABLE     := xsct
COMPILER       := gcc
COMPILER_FLAGS := -std=c11 -Wall -pedantic -Wextra
LINKER_FLAGS   := -lX11 -lXrandr -lm


all: build


build: $(EXECUTABLE)

-include $(OBJECT_FILES:.o=.d)

$(EXECUTABLE): $(OBJECT_FILES)
	$(COMPILER) -o $@ $^ $(LINKER_FLAGS)

$(BUILD_FOLDER)/%.o: %.c
	@mkdir -p $(@D)
	$(COMPILER) -c $(COMPILER_FLAGS) -o $@ $< -MMD -MF $(@:.o=.d)


run: $(EXECUTABLE)
	./$(EXECUTABLE)


clean:
	$(RM) -rf $(BUILD_FOLDER)

.PHONY: all build run clean
