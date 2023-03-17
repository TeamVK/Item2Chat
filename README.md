# Item2Chat

NOTE: for v7.0.0 and up please make sure to use ProtocolLib 5.0.0 or up!!!

Yes, this is yet another Item to chat plugin. We made this because people requested an NMS version-independent one.

This plugin will allow you to insert a popup for the keyword specified in the config.yml (default keyword is "[item]", "[inv]").  When a player hovers over the world "[item]" in the chat, they can see the detail of the item you were holding, or "[inv]" will let you see others your inventory.

### Sample Images:

#### With RGB support:

[MEDIA=youtube]mEJR4ZLRVdg[/MEDIA]

### Command:
 * /item2chat help : displays the help menu
 * /item2chat reload : reloads the config.yml

### Permission:
 * item2chat.use.item : allows you to use the registered keyword ([item]) to show off the item you're holding.
 * item2chat.use.inv : allows you to use the registered keyword ([inv]) to show off your inventory.
 * item2chat.reload : allows you to use the reload command.
 * item2chat.cooldown_bypass : allows you to bypass the cool down limit.

### Installation:
You must install ProtocolLIb first, then you just put Item2Chat.jar file into your server's plugins folder.  If you wish to use placeholders (supported by PlaceholderAPI) in the prefix, please install PlaceholderAPI as well.

### Configuration:
># +------------------------------------------------------------+ #
># Item2Chat Configuration
># +------------------------------------------------------------+ #
>
># NOTE: Do NOT put tabs anywhere in the config!
>
>Messages:
>  ErrorMsg : "&c[Item2Chat] : Some error occured."
>  NoItem: "&c[Item2Chat] : You must have something in your hand to use Item2Chat!"
>  NoPermission: "&c[Item2Chat] : You don't have a permission."
>  CoolDown: "&c[Item2Chat] You have to wait for &b%remaining% &aseconds."
>  LetsOpenSnapshot: "&a[Item2Chat] Let's open %player%'s inventory snapshot!."
>  SnapshotExpired: "&c[Item2Chat] %player%'s inventory snapshot has expired!"
>
>HelpMessages:
  banner:
    msg: "=== &e[&aItem2Chat Commands List (%version%)&e] &r==="  
  help:
    msg: "&a/item2chat help : displays this help menu."
  reload:
    msg: "&a/item2chat reload : reloads config file."
    permission: "item2chat.reload"
  debug:
    msg: "&a/item2chat debug <on|off> : turn on / off the debug mode."
    permission: "item2chat.debug"

CommandAliases:
  item2chat:
    - "i2c"

# this option is for the target outlet of the messages to go. Previously, they were all sent to chat.
MessageOutlet:
  Title: false
  SubTitle: false
  ActionBar: false
  Chat: true

# if this option is true [AIR] will be display when you're not holding any item.
DisplayEmptyHand: false

#if this option is true, the plguin will try to send the chat packet in asynchronous fashion
AsynchronousMode: false

# if you encounter any issue with your chat plugin, try adjusting this option.
# adjust these event priority if those event processes from this plugin
# interfere with other plugins' event processes.
EventPriorityMap:
  AsyncPlayerChatEvent: "LOWEST"
  PlayerCommandPreprocessEvent: "LOWEST"
  PacketEvent: "LOWEST"

Cooldown: 10  # in seconds
CaseSensitive: false
ItemKeyword:
  - "[item]"
  - "{item}"
  - "{i}"

InlineFormat: "&r&f[%name%%INLINE_AMOUNT%&r&f]"
InlineAmountFormat: " (x%amount%)"

# if inventory keyword is used, the inventory snapshot will be kept for the
# following duration (in ticks)
RetainSnapshot: 300 # in ticks

# to use the below feature, you need OpenInv plugin installed on your server.
InvTooltip: "&aClick this to see &e%player_name%&a\\'s inventory"
InvTitle: "%player_name%'s inventory"
InvInline: "%player_name%'s inventory"
InvKeyword:
  - "[inventory]"
  - "{inventory}"
  - "[inv]"
  - "{inv}"
  - "[brag]"
  - "{brag}"

Donation:
It would be greatly appreciated for your donation to continue providing support for this plugin.
