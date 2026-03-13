# Google Voice API

Google Voice is a telecommunications service by Google that provides call forwarding, voicemail, text messaging, and voice calling for personal and Google Workspace business accounts. While Google Voice does not offer an official standalone REST API, voice services can be managed programmatically through the Google Workspace Admin SDK for provisioning users, assigning numbers, and managing locations. Google Voice integrates with Google Workspace for enterprise telephony management.

## Artifacts

- **APIs.yml** - Machine-readable API metadata following the APIs.json specification.
- **OpenAPI** (`openapi/openapi.yml`) - OpenAPI 3.1.0 specification describing the available management endpoints through Google Workspace Admin SDK.
- **JSON Schema** (`json-schema/google-voice.json`) - JSON Schema (draft 2020-12) defining user, building, and voice settings objects.
- **JSON-LD** (`json-ld/google-voice.jsonld`) - JSON-LD context mapping Voice-related terms to schema.org and API-specific vocabularies.

## Key Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/admin/directory/v1/users` | List users with Voice assignments |
| GET | `/admin/directory/v1/users/{userKey}` | Get user details |
| GET | `/admin/directory/v1/customer/{customerId}/resources/buildings` | List buildings for location assignment |

## Note

Google Voice does not currently provide an official standalone public REST API. The endpoints documented here are part of the Google Workspace Admin SDK, which provides the closest programmatic access to managing Google Voice services in an enterprise context.

## Resources

- [Google Voice](https://voice.google.com)
- [Google Voice Help](https://support.google.com/voice)
- [Google Workspace Admin SDK](https://developers.google.com/admin-sdk)
- [Google Voice for Workspace Pricing](https://workspace.google.com/products/voice/)

## Maintainer

Kin Lane - kin@apievangelist.com
