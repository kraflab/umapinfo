# UMAPINFO Rev 2.2

UMAPINFO is a cross-port (universal) MAPINFO variant that allows authors to adjust various aspects of levels and level progression. This includes names, music, par times, related images, episodic structure, secret exit destinations, etc.

The full specification is available [here](./docs/spec.md).

### Revision History

- Rev 2.2 (@rfomin, December 27 2022)
  - Introduce the new `author` field.

- Rev 2.1 (@rfomin, June 22 2021)
  - Lookup for default backdrop if `interbackdrop` is not specified.

- Rev 2 (@fabiangreffrath, May 11 2021)
   - Introduce the new `label` field to allow for overriding of the string that gets prepended to the `levelname` on the automap.

- Rev 1.6 (@fabiangreffrath, Apr 19 2021)
  - Skip the 'entering level' screen if one of `endgame`, `endpic`, `endbunny` or `endcast` is set.

- Rev 1.5 (@Shadow-Hog, Apr 17 2021)
  - Add in all the additional actor names for DEHEXTRA.

- Rev 1.4 (@rfomin, Mar 23 2021)
  - Clarify the `episode` field in the case of Doom 2 and Chex Quest.

- Rev 1.3 (@fabiangreffrath, Mar 5 2021)
  - If `interbackdrop` does not specify a valid flat, draw it as a patch instead.

- Rev 1.2 (@JadingTsunami, Feb 12 2021)
  - Fix typo in ZDoom-style Actor name.

- Rev 1.1 (@XaserAcheron, Jan 24 2021)
  - Updates to the UMAPINFO docs to disambiguate the `bossaction` field a bit.

- Rev 1 (@coelckers, Jul 10 2017)
  - Updated UMAPINFO spec to curly brace syntax.

- Rev 0 (@coelckers, Apr 22 2017)
  - Initial implementation.
