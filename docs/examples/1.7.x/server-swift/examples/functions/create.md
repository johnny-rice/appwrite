import Appwrite
import AppwriteEnums

let client = Client()
    .setEndpoint("https://<REGION>.cloud.appwrite.io/v1") // Your API Endpoint
    .setProject("<YOUR_PROJECT_ID>") // Your project ID
    .setKey("<YOUR_API_KEY>") // Your secret API key

let functions = Functions(client)

let function = try await functions.create(
    functionId: "<FUNCTION_ID>",
    name: "<NAME>",
    runtime: .node145,
    execute: ["any"], // optional
    events: [], // optional
    schedule: "", // optional
    timeout: 1, // optional
    enabled: false, // optional
    logging: false, // optional
    entrypoint: "<ENTRYPOINT>", // optional
    commands: "<COMMANDS>", // optional
    scopes: [], // optional
    installationId: "<INSTALLATION_ID>", // optional
    providerRepositoryId: "<PROVIDER_REPOSITORY_ID>", // optional
    providerBranch: "<PROVIDER_BRANCH>", // optional
    providerSilentMode: false, // optional
    providerRootDirectory: "<PROVIDER_ROOT_DIRECTORY>", // optional
    specification: "" // optional
)

