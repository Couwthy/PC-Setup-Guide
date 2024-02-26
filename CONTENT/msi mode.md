# MSI Mode

- Enable MSI where it is supported (careful with Sata/NVME) (check the sound checkbox). Do not uncheck Sata/NVME/USB, the blue screen will eat you up. Next, set High Priority on the card, USB hub with mouse and their PCI slots, as well as the Internet. Next, delete all values in the Limit column, or enter 256 or 2048. This will remove the limits from the devices. BUT! Not all devices need to have their limits removed. It is better to set limit 1 for Internet and GPU.
