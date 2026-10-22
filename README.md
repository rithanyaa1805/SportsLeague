# SportsLeague
# Sports League & Match Scheduling (Question 23)

## Requirements
- Java JDK 8 or later (Java 8+ is sufficient for this source).
- Eclipse IDE for Java Developers.

## Open in Eclipse
1. Open Eclipse and select a workspace.
2. Choose **File > New > Java Project**.
3. Project name: `SportsLeagueProject`, then click **Finish**.
4. In Package Explorer, expand `SportsLeagueProject > src`.
5. Right-click `src` > **New > Class**.
6. Class name: `SportsLeagueApp`. Tick **public static void main(String[] args)** if shown, then click **Finish**.
7. Open the generated `SportsLeagueApp.java`, select all and replace it with the full contents of the supplied `SportsLeagueApp.java` file. Save with **Ctrl+S**.
8. Right-click `SportsLeagueApp.java` > **Run As > Java Application**.
9. The output appears in the **Console** tab.

Alternative: create the Java project and copy `SportsLeagueApp.java` into the project's `src` folder using File Explorer, then refresh the project in Eclipse (right-click project > Refresh).

## Menu
1. Add Team
2. Add Player
3. Create Fixture
4. Record Match / Update Result
5. View Fixtures and Results
6. View Standings
7. View Disciplinary Log / Add Record
8. Exit

Three sample teams are loaded at startup: Falcons, Tigers, Warriors.

## Fixture date/time format
Enter exactly `yyyy-MM-dd HH:mm`, for example `2026-11-05 16:30`.

## Suggested test run for screenshots
1. Run the app. Capture the initial menu and demo teams.
2. Choose `3` and create a fixture:
   - Home team ID: `1`
   - Away team ID: `2`
   - Date/time: `2026-11-05 16:30`
3. Choose `3` again and try a clash:
   - Home team ID: `1`
   - Away team ID: `3`
   - Date/time: `2026-11-05 16:30`
   - Expected: scheduling clash error; app remains running.
4. Choose `4`, fixture ID `1`, scores `2` and `1`.
5. Choose `6` to show updated standings.
6. Choose `7`, then `1`, team ID `1`, player ID `0` if no player is registered (team-level record), action `Penalty`, details `Unsporting conduct`; or add a player first and record a card against them.
7. Choose `5` to show fixture and result output.
8. Capture the Console after each required output. Use Windows Snipping Tool (`Win + Shift + S`) and save screenshots.

## Screenshot requirements
Your assignment asks for screenshots from the Eclipse Console showing:
- Main menu
- Input validation/error handling (the fixture clash is a useful example)
- Fixture and match result
- Updated league standings
- Disciplinary log

For a clean screenshot, maximize Eclipse, make the Console wide enough to show each line, and take separate screenshots for different menu actions. Do not submit fabricated screenshots; run the program and capture the real Console.

## Notes
This is a single-file version for easier beginner setup. It includes all required class names as separate top-level classes in one `.java` file. It demonstrates encapsulation, aggregation (teams contain players), object relationships between fixtures/matches/results, and standings calculated from recorded results.
