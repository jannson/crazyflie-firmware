################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include utils/src/subdir.mk
-include modules/src/subdir.mk
-include lib/STM32F10x_StdPeriph_Driver/src/subdir.mk
-include lib/FreeRTOS/portable/MemMang/subdir.mk
-include lib/FreeRTOS/portable/GCC/ARM_CM3/subdir.mk
-include lib/FreeRTOS/subdir.mk
-include lib/CMSIS/Core/CM3/subdir.mk
-include init/subdir.mk
-include hal/src/subdir.mk
-include drivers/src/subdir.mk
-include bin/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: crazyflie-firmware

# Tool invocations
crazyflie-firmware: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: Cross GCC Linker'
	arm-none-eabi-gcc  -o "crazyflie-firmware" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(OBJS)$(C_DEPS)$(EXECUTABLES) crazyflie-firmware
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
