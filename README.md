# Item2Chat

NOTE: for v7.0.0 and up please make sure to use ProtocolLib 5.0.0 or up!!!

Yes, this is yet another Item to chat plugin. We made this because people requested an NMS version-independent one.

This plugin will allow you to insert a popup for the keyword specified in the config.yml (default keyword is "[item]", "[inv]").  When a player hovers over the world "[item]" in the chat, they can see the detail of the item you were holding, or "[inv]" will let you see others your inventory.

### Sample Images:

#### With RGB support:
![RGB support](./images/rgb_image.png?raw=true "RGB support")

#### Video demo:
[![Demo](https://img.youtube.com/vi/mEJR4ZLRVdg/0.jpg)](https://youtu.be/mEJR4ZLRVdg)

#### Sample screenshots:
![RGB support](./images/item_keyword.png?raw=true "Keyword")![RGB support](./images/chat_image0.png?raw=true "Lapis")
![RGB support](./images/tooltip.png?raw=true "Tooltip")

![RGB support](./images/chat_image.png?raw=true "dpick")![RGB support](./images/enchant_list.png?raw=true "list")

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

