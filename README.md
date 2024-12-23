# IoT Community Sensors Directory

This repository serves as the primary data store for the IoT Community sensors directory and their companion devices, accessible at [iotCommunity.space/sensors](https://iotCommunity.space/sensors).

## Overview

The IoT Community Sensors Directory is a comprehensive database of IoT sensors and companion devices used across various IoT projects and implementations. This repository maintains the data structure and information that powers the directory website.

## Data Structure

The sensor data is stored in a single `sensors.json` file with the following structure:

```json
{
  "Sensor Name": {
    "Description": "Detailed sensor description",
    "Communication": "Communication protocol used",
    "Applications": ["Application 1", "Application 2"],
    "Environmental Compatibility": "Usage environment details",
    "Data Formats": ["Format 1", "Format 2"],
    "Technology": "Underlying technologies",
    "Cost": "Cost category",
    "Vendor": "Manufacturer name",
    "imageUrl": "URL to sensor image (optional)"
  }
}
```

### Required Fields

Each sensor entry must include:
- Description
- Communication
- Applications (array)
- Environmental Compatibility
- Data Formats (array)
- Technology
- Cost
- Vendor

The `imageUrl` field is optional but recommended.

## Contributing

To add or update sensor information:

1. Fork this repository
2. Create a new branch (`git checkout -b add-new-sensor`)
3. Modify the `sensors.json` file following the data structure above
4. Validate your JSON before submitting
5. Submit a Pull Request

### Example Entry

```json
"LHT65N-VIB -- LoRaWAN Vibration Sensor": {
  "Description": "LoRaWAN protocol for detecting vibration and runtime. Includes temperature & humidity sensors.",
  "Communication": "LoRaWAN",
  "Applications": ["Smart Agriculture", "Industrial Monitoring"],
  "Environmental Compatibility": "Outdoor use, IP-rated",
  "Data Formats": ["JSON", "MQTT"],
  "Technology": "LoRaWAN End node",
  "Cost": "Affordable",
  "Vendor": "Dragino",
  "imageUrl": "https://dragino.com/media/k2/items/cache/3abb66d58aa91d2b7b16f08ee38a95c0_L.jpg"
}
```

## Data Validation

We provide a JSON schema for validating sensor entries. All submissions must pass schema validation before being accepted.

## API Access

The sensor directory data is available through our REST API at `https://iotCommunity.space/sensors/api`. The API returns data in the same JSON structure as shown above.

## License

This repository and its contents are licensed under the MIT License. See [LICENSE](LICENSE) file for details.

## Contact

For questions, suggestions, or support:
- [Join our Discord Community](https://iotCommunity.space/discord)
- [Submit an Issue](https://github.com/iotCommunity/sensors/issues)
- Email: support@iotCommunity.space

## Additional Resources

For more information about the IoT Community and our projects, please visit:
- [Project About Page](https://iotCommunity.space/about)
- [Developer Documentation](https://docs.iotCommunity.space)
- [Community Guidelines](https://iotCommunity.space/guidelines)
