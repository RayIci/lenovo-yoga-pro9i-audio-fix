# Lenovo Yoga fix bassless audio issue

This script temporaneally fix bassless audio issue on lenovo yoga laptops.

## How to use

To fix basseless audio problem in lenovo yoga you have to run the script `2pa-byps.sh`.

First of all you have to install `i2cset` in your system using your package manager 

Ubuntu:

``` bash
sudo apt install i2cset
```

Fedora:

```bash
sudo dnf install i2cset
```

After installing i2cset, make the script executable

```bash
sudo chmod +x ./2pa-byps.sh
```

After that run the script in sudo mode with an argument specifing the channel to bypas, for exaple:

```bash
sudo ./2pa-bypas.sh 2
```

If the script print a failed write change the channel. The script is run succesfully if no failure writing are displayed.

## References

This script has been found in the [following github issue](https://github.com/karypid/YogaPro-16IMH9/issues/2), read the issue to better details.
