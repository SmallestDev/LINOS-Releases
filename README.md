# LINOS

Releases of **LINOS** (Life Is Not One Shot), an investing strategy game for Windows 10/11. Start with ₩10,000,000 of
play money, read the news and invest in 12 fictional companies across semiconductors, AI, energy, EVs, biotech and
more. Prices move with market phases, interest rates, commodities, consumer spending, sector trends and company news,
and every game generates a brand-new market. Your result is scored on return *and* risk: score = return − max
drawdown × 0.5. Play Free Market (20/50/100 rounds), five Challenges, eight economic Scenarios, a Daily Market, or
Versus matches where everyone gets the exact same market and plays at their own pace. Card-table look with a swirling
backdrop, pixel font and bouncy animations. English by default, Korean in Settings.

## Download
Open the [latest release](../../releases/latest) and download `LINOS-windows-<version>-setup.exe`.

## Updates
The app includes an automatic update system.

A few seconds after LINOS starts it checks this repository for a new version. If there is one, it shows what changed
and asks you; nothing is downloaded until you choose **Install and restart**. The installer is verified against the
app's signing key before it runs, and if anything fails the current version keeps working. Your games, records and
settings are kept. You can turn the check off or check manually in **Settings**.

`latest.json` and the `.sig` file are used by the automatic updater. You don't need to download them.

## Installation
1. Download `LINOS-windows-<version>-setup.exe`
2. Run it. It installs for the current user (no administrator rights) to `%LOCALAPPDATA%\LINOS` and adds a Start menu entry
3. Start **LINOS**. The first start takes a few seconds longer while it sets up its local database

> Windows may show "Windows protected your PC" because the installer isn't code-signed. Choose **More info** → **Run anyway**.

> LINOS uses Microsoft Edge WebView2, which is part of Windows 11 and current Windows 10. If it is missing, the installer downloads it.

## Notes
- Everything runs on your PC: LINOS starts its own small game server and PostgreSQL database in the background and stops them when you close it. No account, no telemetry; the only network access is the update check against this repository.
- Versus with friends: in **Settings → Game server**, one player picks **Host for friends** and shares the address shown; the others pick **Join a server** and enter it. You need to be on the same network, and Windows may ask the host to allow LINOS through the firewall.
- Your games and settings are kept in `%LOCALAPPDATA%\com.smallestdev.linos`. Uninstalling keeps them unless you tick "delete app data".
- All companies, prices and money are fictional. LINOS is a game, not investment advice.
