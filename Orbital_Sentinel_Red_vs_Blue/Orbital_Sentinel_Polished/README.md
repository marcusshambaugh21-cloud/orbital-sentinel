# Operation Orbital Sentinel — Red vs Blue

## Start
Install Node.js, open PowerShell in this folder and run:

```powershell
npm install
$env:PORT=5050; npm start
```

Host opens http://localhost:5050. Other players on the same Wi-Fi open http://HOST_IPV4:5050. Allow Node.js through Windows Firewall on a trusted private network if prompted.

## Rules
- Create a room; players join with its code and select Blue or Red Team.
- Room creator starts once both teams have at least one player. Players must join before match starts.
- One satellite per connected cadet, with no hardcoded player cap.
- Maneuver using the controls. Orbital speed depends on altitude (accelerated for gameplay).
- Target Nearest selects an opposing-team satellite. Friendly-fire engagements are rejected by the server.
- Simulated deorbit works within 1,800 km, costs 5 fuel, and has a 7-second cooldown. Disabled satellites respawn after 30 seconds.
- Debris hazards appear every 30 seconds, with a warning phase and collision penalties.
- Match lasts 13 minutes; combined individual scores determine the winning team.

## Notes
The game is a fictional educational simulation, not a real spacecraft-control or orbital warfare system. The globe and orbital mechanics are simplified. No software-defined player cap exists, but performance depends on server and network capacity.
