XML (eXtensible Markup Language) is a way to store and exchange structured data.
A Parser converts Text into objects
DOCTYPE is where XML variables (entities) are defined.

Example:
<!DOCTYPE cookbook [<!ENTITY mysteryingredient SYSTEM "file:///ingredient.txt">] >
<FirmwareUpdateConfig>
  <Firmware>
    <Version>&mysteryingredient;</Version>
  </Firmware>
</FirmwareUpdateConfig>
