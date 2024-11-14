📦 rfid-integration-system
┣ 📂 src
┃ ┣ 📂 api                    # API layer
┃ ┃ ┣ 📂 controllers         # Request handlers
┃ ┃ ┃ ┣ 📄 rfidController.js
┃ ┃ ┃ ┣ 📄 preparationController.js
┃ ┃ ┃ ┣ 📄 dispatchController.js
┃ ┃ ┃ ┣ 📄 returnController.js
┃ ┃ ┃ ┣ 📄 checkInController.js
┃ ┃ ┃ ┗ 📄 settingsController.js
┃ ┃ ┣ 📂 middleware         # Custom middleware
┃ ┃ ┃ ┣ 📄 auth.js
┃ ┃ ┃ ┣ 📄 errorHandler.js
┃ ┃ ┃ ┣ 📄 validation.js
┃ ┃ ┃ ┗ 📄 rateLimiter.js
┃ ┃ ┣ 📂 routes            # API routes
┃ ┃ ┃ ┣ 📄 rfid.routes.js
┃ ┃ ┃ ┣ 📄 preparation.routes.js
┃ ┃ ┃ ┣ 📄 dispatch.routes.js
┃ ┃ ┃ ┣ 📄 return.routes.js
┃ ┃ ┃ ┣ 📄 checkIn.routes.js
┃ ┃ ┃ ┗ 📄 settings.routes.js
┃ ┃ ┗ 📄 index.js          # API entry point
┃ ┣ 📂 config               # Configuration files
┃ ┃ ┣ 📄 database.js
┃ ┃ ┣ 📄 rfid.config.js
┃ ┃ ┣ 📄 aws.config.js
┃ ┃ ┗ 📄 app.config.js
┃ ┣ 📂 core                 # Core business logic
┃ ┃ ┣ 📂 rfid              # RFID reader integration
┃ ┃ ┃ ┣ 📄 reader.js
┃ ┃ ┃ ┣ 📄 parser.js
┃ ┃ ┃ ┗ 📄 eventHandler.js
┃ ┃ ┣ 📂 export            # Export functionality
┃ ┃ ┃ ┣ 📄 csvExporter.js
┃ ┃ ┃ ┗ 📄 fileHandler.js
┃ ┃ ┗ 📂 integration       # Third-party integration
┃ ┃   ┣ 📄 hireTrackNX.js
┃ ┃   ┗ 📄 ftpClient.js
┃ ┣ 📂 db                   # Database models and migrations
┃ ┃ ┣ 📂 models
┃ ┃ ┃ ┣ 📄 Item.js
┃ ┃ ┃ ┣ 📄 Preparation.js
┃ ┃ ┃ ┣ 📄 Dispatch.js
┃ ┃ ┃ ┣ 📄 Return.js
┃ ┃ ┃ ┣ 📄 CheckIn.js
┃ ┃ ┃ ┗ 📄 Settings.js
┃ ┃ ┣ 📂 migrations
┃ ┃ ┗ 📂 seeds
┃ ┣ 📂 services             # Business logic services
┃ ┃ ┣ 📄 rfidService.js
┃ ┃ ┣ 📄 preparationService.js
┃ ┃ ┣ 📄 dispatchService.js
┃ ┃ ┣ 📄 returnService.js
┃ ┃ ┣ 📄 checkInService.js
┃ ┃ ┗ 📄 settingsService.js
┃ ┣ 📂 utils                # Utility functions
┃ ┃ ┣ 📄 logger.js
┃ ┃ ┣ 📄 validation.js
┃ ┃ ┣ 📄 errors.js
┃ ┃ ┗ 📄 helpers.js
┃ ┣ 📂 websocket            # Real-time communication
┃ ┃ ┣ 📄 socket.js
┃ ┃ ┗ 📄 events.js
┃ ┗ 📄 app.js               # Application entry point
┣ 📂 client                  # Frontend React application
┃ ┣ 📂 public
┃ ┣ 📂 src
┃ ┃ ┣ 📂 components        # React components
┃ ┃ ┃ ┣ 📂 rfid
┃ ┃ ┃ ┣ 📂 preparation
┃ ┃ ┃ ┣ 📂 dispatch
┃ ┃ ┃ ┣ 📂 return
┃ ┃ ┃ ┣ 📂 checkIn
┃ ┃ ┃ ┗ 📂 settings
┃ ┃ ┣ 📂 hooks             # Custom React hooks
┃ ┃ ┣ 📂 context           # React context
┃ ┃ ┣ 📂 redux             # State management
┃ ┃ ┃ ┣ 📂 actions
┃ ┃ ┃ ┣ 📂 reducers
┃ ┃ ┃ ┗ 📂 store
┃ ┃ ┣ 📂 services         # API services
┃ ┃ ┣ 📂 utils            # Utility functions
┃ ┃ ┗ 📄 App.js
┣ 📂 tests                   # Test files
┃ ┣ 📂 unit
┃ ┣ 📂 integration
┃ ┗ 📂 e2e
┣ 📂 docs                    # Documentation
┃ ┣ 📄 api.md
┃ ┣ 📄 deployment.md
┃ ┗ 📄 development.md
┣ 📂 scripts                 # Build and deployment scripts
┃ ┣ 📄 build.js
┃ ┣ 📄 deploy.js
┃ ┗ 📄 seed.js
┣ 📄 .env.example            # Environment variables template
┣ 📄 .gitignore
┣ 📄 docker-compose.yml      # Docker configuration
┣ 📄 Dockerfile
┣ 📄 package.json
┗ 📄 README.md
