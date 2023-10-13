BUILD_DIR=build
include $(N64_INST)/include/n64.mk

################################################################
#                    Code files and ROM name                   #
################################################################

SRC = main.c


################################################################
#                         Make Commands                        #
################################################################

all: unflexa2.z64


################################################################
#                          Compilation                         #
################################################################

$(BUILD_DIR)/unflexa2.elf: $(SRC:%.c=$(BUILD_DIR)/%.o)

unflexa2.z64: N64_ROM_TITLE="UNFLEXAM2"

clean:
	rm -rf $(BUILD_DIR) unflexa2.z64

-include $(wildcard $(BUILD_DIR)/*.d)

.PHONY: all clean