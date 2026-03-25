# Garmin Apps

Custom watch faces and apps for Garmin smartwatches, built with the [Connect IQ](https://developer.garmin.com/connect-iq/sdk/) platform and Monkey C.

## Motivation

Write personal watch faces and utility apps that can be sideloaded directly onto a Garmin watch, without depending on the Connect IQ Store ecosystem.

## Planned Apps

| App | Description | Status |
|-----|-------------|--------|
| Analog Watch Face | Simple, elegant watch face with hands | Planned |
| Lap Counter | One-button counter for laps, reps, etc. | Planned |
| Motion Logger | Record accelerometer/GPS data for swim stroke analysis | Planned |

## Platform Notes

- **Language:** Monkey C (object-oriented, influenced by C/Java/JavaScript/Python)
- **SDK:** Free Connect IQ SDK with VS Code extension
- **Sideloading:** Build produces a `.prg` file that can be copied to `/GARMIN/APPS/` on the watch via USB -- no store account required
- **Signing:** Apps must be signed with a self-generated RSA 4096-bit key
- **Limitation:** Sideloaded apps cannot use Connect IQ app settings (settings require the Store)

## Getting Started

1. Install the [Connect IQ SDK](https://developer.garmin.com/connect-iq/sdk/)
2. Install the Monkey C extension for VS Code
3. Generate a developer key (RSA 4096-bit)
4. Build the app (`monkeyc` or via VS Code)
5. Connect your watch via USB and copy the `.prg` file to `/GARMIN/APPS/`

## References

- [Connect IQ SDK](https://developer.garmin.com/connect-iq/sdk/)
- [Connect IQ Basics](https://developer.garmin.com/connect-iq/connect-iq-basics/)
- [Monkey C Language Reference](https://developer.garmin.com/connect-iq/monkey-c/)

## Status

Research and planning phase. See `readme.log` for detailed research notes.
