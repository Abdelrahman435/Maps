# Project: Company and User Mapping with Google Maps API

## Overview

This project is a TypeScript-based application that demonstrates the integration of Google Maps API to display markers for dynamically generated companies and users. The app utilizes `faker.js` to create random data for companies and users, including their names, catchphrases, and geographic locations (latitude and longitude). When clicking on a marker, an info window pops up with details about the respective company or user.

## Features

- **TypeScript Integration**: The project is built using TypeScript, ensuring type safety and better code management.
- **Google Maps API**: The map is rendered using Google Maps API, with custom markers added for users and companies.
- **Dynamic Data Generation**: Randomized data is generated using `faker.js` for companies and users, providing unique names, catchphrases, and locations.
- **Custom Info Windows**: Clickable markers show information about the entity (company or user) in a popup window.

## Project Structure

- **`index.ts`**: Main entry point of the app. Initializes the map and adds markers for a user and a company.
- **`CustomMap.ts`**: Handles the Google Maps logic, providing methods to add markers to the map.
- **`Company.ts`**: Defines the `Company` class, which implements the `Mappable` interface. Each company is assigned a name, catchphrase, and location.
- **`User.ts`**: Defines the `User` class, which also implements the `Mappable` interface. Each user is assigned a name and location.
- **`index.html`**: Contains the basic HTML structure with a `<div>` to hold the map.

## How It Works

1. **Google Maps Initialization**: The `CustomMap` class creates a Google Map centered at coordinates (0, 0) with a zoom level of 1.
2. **Adding Markers**: Using the `addMarker` method, markers are added to the map for the `User` and `Company` instances. These markers are positioned based on the generated lat/lng data.
3. **Info Windows**: Clicking on a marker opens an info window that displays either the company’s name and catchphrase or the user's name.

## Technologies Used

- **TypeScript**: Provides type safety and robust development experience.
- **Google Maps API**: Powers the map functionality and marker rendering.
- **Faker.js**: Generates random names, catchphrases, and locations for companies and users.

## Demo

Watch the demo video of the project: [Demo Video](https://drive.google.com/file/d/1RogKP8CJlmAlNu8wPu8oQbeX1xhf2rGJ/view?usp=drivesdk).

## Dependencies

- `faker`: ^5.5.3
- `googlemaps`: ^1.1.3
- `@types/googlemaps`: ^3.43.3
- `typescript`: ^5.6.2
- `@types/faker`: ^6.6.8

## Future Improvements

- Add more customization to marker colors based on specific attributes.
- Implement more dynamic interaction, such as updating or removing markers.
- Allow user input to generate markers instead of relying on random data.
