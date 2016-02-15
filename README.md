This is failing ASP.NET 5 app, which hangs at accepting a client on Linux.

Runtime: `(Stable 4.2.2.30/996df3c Fri Jan 22 00:02:19 UTC 2016)`
Linux: Debian 8 Jessie
Kernel: `Linux netrunnerdevelopment 3.16.0-4-amd64 #1 SMP Debian 3.16.7-ckt20-1+deb8u3 (2016-01-17) x86_64 GNU/Linux`

Steps to reproduce problem:

1. Use `yo` to scaffold web app.
2. Run `dnu restore && dnu build` to resolve dependencies and build app
3. Run `dnx web` to start app.
4. Open any web browser and go to `http://localhost:5000`.x
