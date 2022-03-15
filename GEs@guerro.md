# GEs@guerro
Infos
======
#### Latest version :
https://v4.live.maniaplanet.com/ingame/public/titles/download/GEs@guerro.Title.Pack.gbx

### Tips/Infos :
if you use maniacontrol on CTF servers, the setting S_WeaponType will be override by maniacontrol, it will replace **'** by **"** in the value attribute, this thing can make issue when you restart the server You will have to put the character **'** in place of **"** for it to work

replace :
```xml
<setting name="S_WeaponType" type="text" value="{"Values":[{"Name":"laser", "Gain": 1.4}]}"/> <!-- Default : {"Values":[]} -->
```
by : 
```xml
<setting name="S_WeaponType" type="text" value='{"Values":[{"Name":"laser", "Gain": 1.4}]}'/> <!-- Default : {"Values":[]} -->
```

TrackLists
======


## CTF Rocket only :
```xml
<?xml version="1.0" encoding="utf-8" ?>
<playlist>
	<gameinfos>
		<game_mode>0</game_mode>
		<script_name>CTF\CTFMode.Script.txt</script_name>
		<title>GEs@guerro</title>
		<chat_time>10000</chat_time>
		<finishtimeout>1</finishtimeout>
		<allwarmupduration>0</allwarmupduration>
		<disablerespawn>0</disablerespawn>
		<forceshowallopponents>0</forceshowallopponents>
	</gameinfos>

	<hotseat>
		<game_mode>0</game_mode>
		<time_limit>300000</time_limit>
		<rounds_count>5</rounds_count>
	</hotseat>

	<filter>
		<is_lan>1</is_lan>
		<is_internet>1</is_internet>
		<is_solo>0</is_solo>
		<is_hotseat>0</is_hotseat>
		<sort_index>1000</sort_index>
		<random_map_order>0</random_map_order>
	</filter>

	<mode_script_settings>
		<setting name="S_WeaponType" type="text" value='{"Values": [{"Name": "rocket"}]}'/> <!-- Default : {"Values":[]} -->
		<setting name="S_EnableCompetitive" type="boolean" value="1"/> <!-- Default : 0 -->
		<setting name="S_NbPlayersPerTeamMax" type="integer" value="5"/> <!-- Default : 3 -->
		<setting name="S_TurnsToWin" type="integer" value="2"/> <!-- Default : 1 -->
		<setting name="S_TimeLimit" type="integer" value="480"/> <!-- Default : 300 -->
		<setting name="S_OvertimeLimit" type="integer" value="300"/> <!-- Default : 180 -->
		<!-- Default : <setting name="S_NbPlayersPerTeamMin" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_ChatTime" type="integer" value="10"/> -->
		<!-- Default : <setting name="S_UseClublinks" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_UseClublinksSponsors" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_NeutralEmblemUrl" type="text" value=""/> -->
		<!-- Default : <setting name="S_ScriptEnvironment" type="text" value="production"/> -->
		<!-- Default : <setting name="S_IsChannelServer" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DelayBeforeNextMap" type="integer" value="2000"/> -->
		<!-- Default : <setting name="S_Debug_DisplayChannelProgression" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingAPIUrl" type="text" value="https://v4.live.maniaplanet.com/ingame/public/matchmaking"/> -->
		<!-- Default : <setting name="S_MatchmakingMatchServers" type="text" value=""/> -->
		<!-- Default : <setting name="S_MatchmakingMode" type="integer" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchRatio" type="real" value="-1"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchNbMax" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_MatchmakingVoteForMap" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingProgressive" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingWaitingTime" type="integer" value="20"/> -->
		<!-- Default : <setting name="S_MatchmakingEnablePenalty" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyRoundPerMap" type="integer" value="60"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerPerRound" type="integer" value="6"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerWait" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_LobbyDisplayMasters" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyDisableUI" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyAggressiveTransfer" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_KickTimedOutPlayers" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_MatchmakingErrorMessage" type="text" value="Â’An error occured in the matchmaking API. If the problem persist please try to contact this server administrator."/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIError" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogMiscDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_WaitingTime" type="integer" value="180000"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_PlayersNbRatio" type="integer" value="1"/> -->
		<!-- Default : <setting name="S_AutoManageAFK" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyInstagib" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_FlagCaptureRespawnTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_FlagOnGroundRespawnTime" type="integer" value="12"/> -->
		<!-- Default : <setting name="S_CaptureGainTimeNormal" type="integer" value="50"/> -->
		<!-- Default : <setting name="S_CaptureGainTimeOvertime" type="integer" value="50"/> -->
		<!-- Default : <setting name="S_ExpAttackDefense" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_EnableWarmUp" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_WarmUpDuration" type="integer" value="120"/> -->
		<!-- Default : <setting name="S_ArmorCount" type="integer" value="200"/> -->
		<!-- Default : <setting name="S_EnableTeamDamage" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_CaptureToWin" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_HudModulePath" type="text" value="what"/> -->
	</mode_script_settings>

	<startindex>4</startindex>
	<map>
		<!-- ..... -->
	</map>
	<map>
		<!-- ..... -->
	</map>
</playlist>
```

## CTF Instagib :
```xml
<?xml version="1.0" encoding="utf-8" ?>
<playlist>
	<gameinfos>
		<game_mode>0</game_mode>
		<script_name>CTF\CTFMode.Script.txt</script_name>
		<title>GEs@guerro</title>
		<chat_time>10000</chat_time>
		<finishtimeout>1</finishtimeout>
		<allwarmupduration>0</allwarmupduration>
		<disablerespawn>0</disablerespawn>
		<forceshowallopponents>0</forceshowallopponents>
	</gameinfos>

	<hotseat>
		<game_mode>0</game_mode>
		<time_limit>300000</time_limit>
		<rounds_count>5</rounds_count>
	</hotseat>

	<filter>
		<is_lan>1</is_lan>
		<is_internet>1</is_internet>
		<is_solo>0</is_solo>
		<is_hotseat>0</is_hotseat>
		<sort_index>1000</sort_index>
		<random_map_order>0</random_map_order>
	</filter>

	<mode_script_settings>
		<setting name="S_EnableWarmUp" type="boolean" value="0"/> <!-- Default : 1 -->
		<setting name="S_WeaponType" type="text" value='{"Values":[{"Name":"laser", "Gain": 1.4}]}'/> <!-- Default : {"Values":[]} -->
		<setting name="S_ArmorCount" type="integer" value="100"/> <!-- Default : 200 -->
		<!-- Default : <setting name="S_ChatTime" type="integer" value="10"/> -->
		<!-- Default : <setting name="S_UseClublinks" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_UseClublinksSponsors" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_NeutralEmblemUrl" type="text" value=""/> -->
		<!-- Default : <setting name="S_ScriptEnvironment" type="text" value="production"/> -->
		<!-- Default : <setting name="S_IsChannelServer" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DelayBeforeNextMap" type="integer" value="2000"/> -->
		<!-- Default : <setting name="S_Debug_DisplayChannelProgression" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingAPIUrl" type="text" value="https://v4.live.maniaplanet.com/ingame/public/matchmaking"/> -->
		<!-- Default : <setting name="S_MatchmakingMatchServers" type="text" value=""/> -->
		<!-- Default : <setting name="S_MatchmakingMode" type="integer" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchRatio" type="real" value="-1"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchNbMax" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_MatchmakingVoteForMap" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingProgressive" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingWaitingTime" type="integer" value="20"/> -->
		<!-- Default : <setting name="S_MatchmakingEnablePenalty" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyRoundPerMap" type="integer" value="60"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerPerRound" type="integer" value="6"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerWait" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_LobbyDisplayMasters" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyDisableUI" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyAggressiveTransfer" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_KickTimedOutPlayers" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_MatchmakingErrorMessage" type="text" value="Â’An error occured in the matchmaking API. If the problem persist please try to contact this server administrator."/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIError" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogMiscDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_WaitingTime" type="integer" value="180000"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_PlayersNbRatio" type="integer" value="1"/> -->
		<!-- Default : <setting name="S_AutoManageAFK" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyInstagib" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_TimeLimit" type="integer" value="300"/> -->
		<!-- Default : <setting name="S_FlagCaptureRespawnTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_FlagOnGroundRespawnTime" type="integer" value="12"/> -->
		<!-- Default : <setting name="S_CaptureGainTimeNormal" type="integer" value="50"/> -->
		<!-- Default : <setting name="S_CaptureGainTimeOvertime" type="integer" value="50"/> -->
		<!-- Default : <setting name="S_OvertimeLimit" type="integer" value="180"/> -->
		<!-- Default : <setting name="S_ExpAttackDefense" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_TurnsToWin" type="integer" value="1"/> -->
		<!-- Default : <setting name="S_EnableCompetitive" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_NbPlayersPerTeamMax" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_NbPlayersPerTeamMin" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_WarmUpDuration" type="integer" value="120"/> -->
		<!-- Default : <setting name="S_EnableTeamDamage" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_CaptureToWin" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_HudModulePath" type="text" value="what"/> -->
	</mode_script_settings>

	<startindex>4</startindex>
	<map>
	<!-- ... -->
	</map>

</playlist>
```


## DodgeBall FFA :
```xml
<?xml version="1.0" encoding="utf-8" ?>
<playlist>
	<gameinfos>
		<game_mode>0</game_mode>
		<script_name>DodgeballFun.Script.txt</script_name>
		<title>GEs@guerro</title>
		<chat_time>10000</chat_time>
		<finishtimeout>1</finishtimeout>
		<allwarmupduration>0</allwarmupduration>
		<disablerespawn>0</disablerespawn>
		<forceshowallopponents>0</forceshowallopponents>
	</gameinfos>

	<hotseat>
		<game_mode>0</game_mode>
		<time_limit>300000</time_limit>
		<rounds_count>5</rounds_count>
	</hotseat>

	<filter>
		<is_lan>1</is_lan>
		<is_internet>1</is_internet>
		<is_solo>0</is_solo>
		<is_hotseat>0</is_hotseat>
		<sort_index>1000</sort_index>
		<random_map_order>0</random_map_order>
	</filter>

	<mode_script_settings>
		<setting name="S_PointsLimit" type="integer" value="2"/> <!-- Default : 3 -->
		<setting name="S_MeterPerSecondGain" type="real" value="1"/> <!-- Default : 0.8 -->
		<setting name="S_NextTurnSpeedFactor" type="real" value="0.7"/> <!-- Default : 0.5 -->
		<!-- Default : <setting name="S_ChatTime" type="integer" value="10"/> -->
		<!-- Default : <setting name="S_UseClublinks" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_UseClublinksSponsors" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_NeutralEmblemUrl" type="text" value=""/> -->
		<!-- Default : <setting name="S_ScriptEnvironment" type="text" value="production"/> -->
		<!-- Default : <setting name="S_IsChannelServer" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DelayBeforeNextMap" type="integer" value="2000"/> -->
		<!-- Default : <setting name="S_Debug_DisplayChannelProgression" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingAPIUrl" type="text" value="https://v4.live.maniaplanet.com/ingame/public/matchmaking"/> -->
		<!-- Default : <setting name="S_MatchmakingMatchServers" type="text" value=""/> -->
		<!-- Default : <setting name="S_MatchmakingMode" type="integer" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchRatio" type="real" value="-1"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchNbMax" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_MatchmakingVoteForMap" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingProgressive" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingWaitingTime" type="integer" value="20"/> -->
		<!-- Default : <setting name="S_MatchmakingEnablePenalty" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyRoundPerMap" type="integer" value="60"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerPerRound" type="integer" value="6"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerWait" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_LobbyDisplayMasters" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyDisableUI" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyAggressiveTransfer" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_KickTimedOutPlayers" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_MatchmakingErrorMessage" type="text" value="Â’An error occured in the matchmaking API. If the problem persist please try to contact this server administrator."/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIError" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogMiscDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_WaitingTime" type="integer" value="180000"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_PlayersNbRatio" type="integer" value="1"/> -->
		<!-- Default : <setting name="S_AutoManageAFK" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyInstagib" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DashReflectBall" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DashHalveSpeed" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_GainSpeedOnReflect" type="boolean" value="1"/> -->
	</mode_script_settings>

	<startindex>10</startindex>
	<map>
		<!-- ... -->
	</map>

</playlist>
```


## DodgeBall Team :
```xml
<?xml version="1.0" encoding="utf-8" ?>
<playlist>
	<gameinfos>
		<game_mode>0</game_mode>
		<script_name>DodgeballLifeTeam.Script.txt</script_name>
		<title>GEs@guerro</title>
		<chat_time>10000</chat_time>
		<finishtimeout>1</finishtimeout>
		<allwarmupduration>0</allwarmupduration>
		<disablerespawn>0</disablerespawn>
		<forceshowallopponents>0</forceshowallopponents>
	</gameinfos>

	<hotseat>
		<game_mode>0</game_mode>
		<time_limit>300000</time_limit>
		<rounds_count>5</rounds_count>
	</hotseat>

	<filter>
		<is_lan>1</is_lan>
		<is_internet>1</is_internet>
		<is_solo>0</is_solo>
		<is_hotseat>0</is_hotseat>
		<sort_index>1000</sort_index>
		<random_map_order>0</random_map_order>
	</filter>

	<mode_script_settings>
		<setting name="S_PointsLimit" type="integer" value="2"/> <!-- Default : 3 -->
		<setting name="S_MeterPerSecondGain" type="real" value="1"/> <!-- Default : 0.8 -->
		<setting name="S_NextTurnSpeedFactor" type="real" value="0.7"/> <!-- Default : 0.5 -->
		<setting name="S_WarmUpDuration" type="integer" value="6"/> <!-- Default : 120 -->
		<!-- Default : <setting name="S_ChatTime" type="integer" value="10"/> -->
		<!-- Default : <setting name="S_UseClublinks" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_UseClublinksSponsors" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_NeutralEmblemUrl" type="text" value=""/> -->
		<!-- Default : <setting name="S_ScriptEnvironment" type="text" value="production"/> -->
		<!-- Default : <setting name="S_IsChannelServer" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DelayBeforeNextMap" type="integer" value="2000"/> -->
		<!-- Default : <setting name="S_Debug_DisplayChannelProgression" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingAPIUrl" type="text" value="https://v4.live.maniaplanet.com/ingame/public/matchmaking"/> -->
		<!-- Default : <setting name="S_MatchmakingMatchServers" type="text" value=""/> -->
		<!-- Default : <setting name="S_MatchmakingMode" type="integer" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchRatio" type="real" value="-1"/> -->
		<!-- Default : <setting name="S_MatchmakingRematchNbMax" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_MatchmakingVoteForMap" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingProgressive" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingWaitingTime" type="integer" value="20"/> -->
		<!-- Default : <setting name="S_MatchmakingEnablePenalty" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyRoundPerMap" type="integer" value="60"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerPerRound" type="integer" value="6"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerWait" type="integer" value="2"/> -->
		<!-- Default : <setting name="S_LobbyMatchmakerTime" type="integer" value="8"/> -->
		<!-- Default : <setting name="S_LobbyDisplayMasters" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_LobbyDisableUI" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyAggressiveTransfer" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_KickTimedOutPlayers" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_MatchmakingErrorMessage" type="text" value="Â’An error occured in the matchmaking API. If the problem persist please try to contact this server administrator."/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIError" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogAPIDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_MatchmakingLogMiscDebug" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_WaitingTime" type="integer" value="180000"/> -->
		<!-- Default : <setting name="S_ProgressiveActivation_PlayersNbRatio" type="integer" value="1"/> -->
		<!-- Default : <setting name="S_AutoManageAFK" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_LobbyInstagib" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DashReflectBall" type="boolean" value="0"/> -->
		<!-- Default : <setting name="S_DashHalveSpeed" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_GainSpeedOnReflect" type="boolean" value="1"/> -->
		<!-- Default : <setting name="S_ArmorCount" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_NbPlayersPerTeamMax" type="integer" value="3"/> -->
		<!-- Default : <setting name="S_NbPlayersPerTeamMin" type="integer" value="1"/> -->
	</mode_script_settings>

	<startindex>5</startindex>
	<map>
		<!-- ... -->
	</map>

</playlist>
```