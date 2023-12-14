sequenceDiagram
  participant User
  participant Device

  User ->> Device: Power on
  Device ->> User: Device initialized
  Device ->> User: Display main menu

  User ->> Device: Select "Move fiber"
  Device ->> User: Control stepper motor with joystick
  Device ->> User: Update fiber position on OLED display

  User ->> Device: Select "Change settings"
  Device ->> User: Adjust device settings through menu options

  User ->> Device: Select "Exit"
  Device ->> User: Turn off device
