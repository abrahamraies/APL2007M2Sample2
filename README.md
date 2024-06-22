
# Cheese Cave Monitoring System

This project is a .NET 6 application designed for monitoring environmental conditions in a cheese cave, specifically temperature and humidity, using a BME280 sensor. The application collects data from the sensor and sends telemetry to the cloud for analysis and monitoring. It's part of the "Accelerate App Development with GitHub Copilot" initiative.

## Features

- **Environment Monitoring**: Measures temperature and humidity using the BME280 sensor.
- **Cloud Integration**: Sends telemetry data to the cloud at specified intervals for remote monitoring.
- **GPIO Control**: Utilizes the GPIO pins of the device for sensor communication.

## Prerequisites

- .NET 6 SDK
- A device with GPIO pins (e.g., Raspberry Pi)
- BME280 sensor module
- Microsoft Azure account (for cloud telemetry)

## Getting Started

1. **Clone the Repository**

    ```sh
    git clone https://github.com/yourusername/cheese-cave-monitoring.git
    ```

2. **Navigate to the Project Directory**

    ```sh
    cd cheese-cave-monitoring
    ```

3. **Restore NuGet Packages**

    Ensure all required NuGet packages are restored by running:

    ```sh
    dotnet restore
    ```

4. **Build the Project**

    Compile the project using:

    ```sh
    dotnet build
    ```

5. **Run the Application**

    Start the application with:

    ```sh
    dotnet run
    ```

## Configuration

- **Sensor Pins**: Configure the GPIO pin used by the BME280 sensor in `Program.cs`.
- **Cloud Settings**: Set up your cloud endpoint and authentication in `Program.cs` for telemetry data.

## Dependencies

- `Microsoft.Azure.Devices.Client` for cloud communication.
- `System.Device.Gpio` for GPIO control.
- `Iot.Device.Bmxx80` for BME280 sensor operations.
- `Newtonsoft.Json` for JSON serialization.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue for further discussion.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.