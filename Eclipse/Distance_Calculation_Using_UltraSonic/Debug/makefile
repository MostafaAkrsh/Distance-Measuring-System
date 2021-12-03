################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(ASM_DEPS)),)
-include $(ASM_DEPS)
endif
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 
LSS += \
Distance_Calculation_Using_UltraSonic.lss \

SIZEDUMMY += \
sizedummy \


# All Target
all: Distance_Calculation_Using_UltraSonic.elf secondary-outputs

# Tool invocations
Distance_Calculation_Using_UltraSonic.elf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: AVR C Linker'
	avr-gcc -Wl,-Map,Distance_Calculation_Using_UltraSonic.map -mmcu=atmega16 -o "Distance_Calculation_Using_UltraSonic.elf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '

Distance_Calculation_Using_UltraSonic.lss: Distance_Calculation_Using_UltraSonic.elf
	@echo 'Invoking: AVR Create Extended Listing'
	-avr-objdump -h -S Distance_Calculation_Using_UltraSonic.elf  >"Distance_Calculation_Using_UltraSonic.lss"
	@echo 'Finished building: $@'
	@echo ' '

sizedummy: Distance_Calculation_Using_UltraSonic.elf
	@echo 'Invoking: Print Size'
	-avr-size --format=avr --mcu=atmega16 Distance_Calculation_Using_UltraSonic.elf
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) $(ELFS)$(OBJS)$(ASM_DEPS)$(S_DEPS)$(SIZEDUMMY)$(S_UPPER_DEPS)$(LSS)$(C_DEPS) Distance_Calculation_Using_UltraSonic.elf
	-@echo ' '

secondary-outputs: $(LSS) $(SIZEDUMMY)

.PHONY: all clean dependents
.SECONDARY:

-include ../makefile.targets
