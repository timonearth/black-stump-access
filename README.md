# Black Stump staff access

Implemented in the Unity main scene (S129), ready for Build & Test. It will affect the published world only after that version is uploaded.

## Permanent staff

Edit [staff.txt](https://github.com/timonearth/black-stump-access/edit/main/staff.txt): one exact VRChat display name per line, then Commit changes. Copy the name from VRChat, including special characters. Names are public; do not add private information. List endpoint: https://timonearth.github.io/black-stump-access/staff.txt

Clients load the list on entry and refresh approximately every five minutes. GitHub Pages publishing/caching can add delay. Tim can use REFRESH STAFF on the backstage panel. A failed refresh retains the last successfully loaded list; a new client with no successful download has only the in-world fallback. Tim's existing owner access remains available offline.

## Guest passes for this instance

Only timonearth sees the BACKSTAGE ACCESS panel beside the backstage cave controls, near the staff arrival point. Use PREVIOUS/NEXT to choose a person, then GRANT PASS. They can use the alley staff door or either stage-side staff entrance.

A pass remains valid if Tim leaves or the guest disconnects and rejoins the same active instance. It is not permanent and does not carry into a new instance. Use REVOKE PASS to remove it; offline grantees remain selectable. Revoke does not remove permanent staff status. Guests do not gain permission to manage access or operate the wardrobe gate.

These lists match display names; they are not VRChat group roles or server-side security. Keep names current. Two-client ownership migration and late-join synchronization still need a real VRChat test; ClientSim grant/revoke, reconnect retention and permission checks passed.