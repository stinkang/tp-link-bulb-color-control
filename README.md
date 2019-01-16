# tp-link-bulb-color-control

## Control a TP-Link color changing bulb with this program. 
This was used to randomly change the color of a KL130 model bulb for a set number of seconds.

# Usage

1. Edit the `USERNAME` and `PASSWORD` variables to your corresponding TP-Link account username and password. 
2. Change the `appType` parameter to the correct one ("Kasa_Android" or "Kasa_iOS").
3. From the command line, create a TpLinkApiTests object `obj`.
4. Run `obj`'s `test_change_bulb_colour()` method. You should see the bulb change once to a random color.
   Note the three lines it prints out before the response message. The first is the `app_server_url`, the second is 
   `device_id` and the third is `token`.
5. Run `obj`'s `countinuously_change_bulb_color()` method with four parameters: the number of seconds between transitions,
   `app_server_url`, `device_id`, and `token`. You should now see the console outputting the response messages as the bulb
   changes color every `seconds` seconds.
6. To stop the process, use Ctrl-C or Command-C from the command line.
