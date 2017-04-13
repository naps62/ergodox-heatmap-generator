# Ergodox heatmap generator

This is my own generator for a heatmap of my [Ergodox] usage.

Data is fed via real-time data collected via [`hid_listen`], and stored in
a SQlite3 database.

This is running in my system as a systemd job, with another script that I can
manually run to grab the counters from the database and generate a heatmap from
an SVG template.

Here's how it looks after about 5 minutes of keyboard usage:

![example.svg](Example heatmap)

## Disclaimer

This was hacked in a single day to work for my use case. There are many loose
ends, particularly regarding systemd setup and installation.

I'll gladly accept Pull requests to improve on this, but for now, and since it's
already working for me, I probably won't update this that much unless I need to.

## License

I don't even care
