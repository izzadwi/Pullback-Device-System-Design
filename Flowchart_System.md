graph TD
 Start
 IsPowerConnected{Is power connected?}
 Start --> IsPowerConnected
 IsPowerConnectedYes --> InitializeDevice
 InitializeDevice --> DisplayMainMenu
 IsPowerConnectedNo --> ConnectPowerOrReplaceBattery
 ConnectPowerOrReplaceBattery --> Start
 DisplayMainMenu
 SelectOptionFromMainMenu{Select option from main menu}
 DisplayMainMenu --> SelectOptionFromMainMenu
 SelectOptionFromMainMenuMoveFiber --> ControlStepperMotorWithJoystick
 ControlStepperMotorWithJoystick --> UpdateFiberPositionOnOLEDDisplay
 SelectOptionFromMainMenuChangeSettings --> AdjustDeviceSettingsThroughMenuOptions
 SelectOptionFromMainMenuExit --> TurnOffDevice
 TurnOffDevice --> Start
 End
 TurnOffDevice --> End
