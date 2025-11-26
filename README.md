Xcode Cloud Workflow

1) Register App identifier on Apple Developer Account (https://developer.apple.com/)
2) Create new App on Appstore Connect (https://appstoreconnect.apple.com/)
3) Open Git Repository project on Xcode 
4)  Go to the Report navigator (⌘ + 9), and press Get Started… under the Cloud tab. If you’ve already created a workflow, you may instead right-click on the target and choose Manage Workflows… to create a new one.
5) Xcode will guide you through creating a new workflow, starting with selecting the target you want to use. Most configuration is done on the Review Workflow page. Press Edit Workflow… on the bottom of the sheet.
6) In the environment settings, enable the Clean option to build every deployment from scratch. This is a requirement by Xcode Cloud when building for Release.
7) Add a new start condition based on Tag Changes and remove the one based on branch. You can configure the start conditions even further by for instance requiring the commit to be tagged with a certain tag Or start condition based on branch
8) In the archive settings you want to select App Store as the Deployment Preparation. If you have TestFlight enabled, you may select Test Flight alternatives here after you have created the workflow.
9) Press save and proceed to the next step of granting access and connecting the workflow to your GitHub repository.
