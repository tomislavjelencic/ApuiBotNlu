# ApuiBotNlu

Bot Framework v4

## Prerequisites

### Install .NET Core

- [.NET Core SDK](https://dotnet.microsoft.com/download) version 3.1

### Create a LUIS Application for NLU

The LUIS model: `CognitiveModels/FlightBooking.json`

[LUIS NLU](https://www.luis.ai)
Login > New authoring service > New app > Import as JSON > Upload `CognitiveModels/FlightBooking.json` > Train > Publish

Add to appsettings.json:

{
    "LuisAppId": "add",
    "LuisAPIKey": "add",
    "LuisAPIHostName": "add"
}

## To try

- In a terminal, navigate to `ApuiBotNlu`

    ```bash
    # change into project folder
    cd ApuiBotNlu
    ```

- Run the bot from a terminal or from Visual Studio, choose option A or B.

  A) From a terminal

  ```bash
  # run the bot
  dotnet run
  ```

  B) Or from Visual Studio

  - Launch Visual Studio
  - File -> Open -> Project/Solution
  - Navigate to `ApuiBotNlu` folder
  - Select `ApuiBotNlu.csproj` file
  - Press `F5` to run the project

## Testing the bot using Bot Framework Emulator

Install [Bot Framework Emulator](https://github.com/microsoft/BotFramework-Emulator/releases/tag/v4.14.1)

- Launch Bot Framework Emulator
- Open Bot
- Enter a Bot URL of `http://localhost:3978/api/messages`

### Test APUI NLU bot

Ask:

Book a flight from New York to Berlin on April 18, 2022

Hello I would like to book a flight for the 7th March of 2022 from Berlin to New York	

I would like to fly to Paris on April 16th 2022


