################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include src/subdir.mk
-include SDK/S32K144_SDK_4.0.1/platform/drivers/src/pins/subdir.mk
-include SDK/S32K144_SDK_4.0.1/platform/drivers/src/interrupt/subdir.mk
-include SDK/S32K144_SDK_4.0.1/platform/drivers/src/clock/S32K1xx/subdir.mk
-include SDK/S32K144_SDK_4.0.1/platform/devices/S32K144/startup/subdir.mk
-include SDK/S32K144_SDK_4.0.1/platform/devices/subdir.mk
-include Project_Settings/Startup_Code/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
SECONDARY_SIZE += \
Mock_Project.siz \


# All Target
all: Mock_Project.elf secondary-outputs

# Tool invocations
Mock_Project.elf: $(OBJS) C:/fpt/MCU/workspace/Mock_Project/Project_Settings/Linker_Files/S32K144_64_flash.ld $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: Standard S32DS C Linker'
	arm-none-eabi-gcc -o "Mock_Project.elf" "@Mock_Project.args"  $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '

Mock_Project.siz: Mock_Project.elf
	@echo 'Invoking: Standard S32DS Print Size'
	arm-none-eabi-size --format=berkeley Mock_Project.elf
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) ./*
	-@echo ' '

secondary-outputs: $(SECONDARY_SIZE)

.PHONY: all clean dependents

-include ../makefile.targets
