# webRTC Video Chat .net Core 3.1 Angular 9
Test project using SignalR on .net Core 3.1 as WebRTC server. Using Angular 9 for managing the connection between 2 peers and connecting to backend for initializing the WebRTC

## Development server
### backend
  ```bash
  cd backend
  dotnet restore
  dotnet run
  ```
It will create dev environment on `http://localhost:5000/`, for all webRTC requests.
### frontend
```bash
cd frontend
npm install
ng serve
``` 
For a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Build prod
### backend
```bash
dotnet restore
dotnet build
dotnet publish
```
Build will create a final version on `backend\bin\Debug\netcoreapp3.1\publish\` that you can use by executing `signalrtc.exe` or `dotnet signalrtc.dll` depending on your environment

### frontend
```bash
npm install
ng build --prod
```
The build artifacts will be stored in the `dist/` directory.
