# ui-utils
Dupe hunting mod for 1.19.2.

---

- How to use:

- Open any inventory/container with the mod and you should see a few buttons.

- [image](https://user-images.githubusercontent.com/85349822/187423033-46da8cc0-2bc3-4215-8676-7c03628b8b8c.png)

- "Close without packet" closes your current gui (ScreenHandler) without sending a `CloseHandledScreenC2SPacket` to the server.

- "De-sync" closes your current gui server-side and keeps it open client-side.

- "Send packets: ???" tells the client whether it should send any `ClickSlotC2SPacket`(s) and `ButtonClickC2SPacket`(s).

- "Delay packets: ???" when turned on it will store all `ClickSlotC2SPacket`(s) and `ButtonClickC2SPacket`(s) into a list and will not send them immdiately until turned off which sends them all at once.

- "Save GUI" saves your current gui to a variable and can be accessed by pressing a keybind in the keybinding options (default key is 'V').

- "Disconnect and send packets" will if "Delay packets" is turned on send the list of stored packets immediately and then disconnect right afterward (can create potential race conditions on non-vanilla servers).

- "Sync Id: ??" is a number used interally to sync various gui related packets.

- "Revision: ??" is a number used interally to sync various gui related packets sent from the server to the client.

- "Fabricate packet" allows you to create a custom `ClickSlotC2SPacket` and `ButtonClickC2SPacket` within a window it creates.

- Fabricate packet tutorial:
---