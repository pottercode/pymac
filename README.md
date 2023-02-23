# Pymac

A MAC address oriented clipboard manipulator for Python 3.9

# Description

Searches your Windows clipboard for MAC addresses, reformats them as instructed, and overwrites the clipboard with a list of the formatted MAC addresses.

Currently recognizes and can convert between four MAC address formats:
    * Colon-separated MAC (A1:B2:C3:D4:E5:F6)
    * Hyphen-separated MAC (A1-B2-C3-D4-E5-F6)
    * period-separated MAC (a1b2.c3d4.e4f6)
    * un-punctuated MAC (A1B2C3D4E5F6)

Purpose: It makes my work a little easier. Maybe it'll do the same for you!
Clients will give you MAC addresses however they feel, but several tools I use only accept a specific format.
This script lets you quickly pull the MACs out of copied text (e.g., an email body), convert them, and paste them out to a .txt file or similar.

# Dependencies

	* pyperclip
	* re
	* argparse

# Arguments

	* -c : Convert detected MACs to colon-separated format.
	* -y : Convert detected MACs to hyphen-separated format.
	* -p : Convert detected MACs to 3x4 period-separated format.
	* -t : Convert detected MACs to un-punctuated format.

# Possible future developments

  * Condense the regex - I'm sure capture groups can tighten this up.
  * Linking to an email pipeline? E.g., process email tickets of the appropriate category and save output to <ticket_number>.txt.
