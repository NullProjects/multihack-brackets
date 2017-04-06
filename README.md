# multihack-brackets
Synchronizes code and project structure between multiple users in realtime.  
Also check out [the web version](https://github.com/RationalCoding/multihack-web). (Now compatible with this extension!)

## Usage
1. You and another person with this extension should have the same project open.  
2. **File > Start Multihack**  
3. Enter the same secret room ID.    
4. Click **Join Room**. Your code is now being synchronized!  
5. **File > Stop Multihack** will stop collaboration.  

This extension currently only syncs *changes* and will not realize any code differences that existed before joining a room.  
To force the extension to pull the code from your peers, do **File > Fetch Code** after joining.  
If peers have different sets of code, the peer who joined first will take priority.  

## Voice Calls
Brackets does not allow microphone access by default. You must launch brackets with:  
`brackets --args --enable-media-stream` if you want to enable voice calls.  

## Running Your Own Instance
This extension points to the author's server by default.  
Please run your own instance of [multihack-server](https://github.com/RationalCoding/multihack-server) if you want lower latency and improved privacy.  
You can target a different host through the Brackets option **multihack-brackets.hostname**.

## Future Features
- [x] Integration with web version
- [ ] Integration with future versions on Atom and VSCode
- [ ] Switch from server forwarding to P2P
- [x] Audio calls
- [ ] Video calls
- [ ] Text chat
- [x] Initial code sync
- [ ] End-to-end encryption
- [ ] Cursor and selection tracking
