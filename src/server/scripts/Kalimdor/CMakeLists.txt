# Copyright (C) 2013-2016 JadeCore <https://www.jadecore.tk/>
#
# This program is free software; you can redistribute it and/or modify it
# under the terms of the GNU General Public License as published by the
# Free Software Foundation; either version 2 of the License, or (at your
# option) any later version.
#
# This program is distributed in the hope that it will be useful, but WITHOUT
# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
# FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
# more details.
#
# You should have received a copy of the GNU General Public License along
# with this program. If not, see <http://www.gnu.org/licenses/>.

set(scripts_STAT_SRCS
  ${scripts_STAT_SRCS}
  Kalimdor/RazorfenDowns/razorfen_downs.cpp
  Kalimdor/RazorfenDowns/instance_razorfen_downs.cpp
  Kalimdor/RazorfenDowns/boss_amnennar_the_coldbringer.cpp
  Kalimdor/RazorfenDowns/razorfen_downs.h
  Kalimdor/ZulFarrak/zulfarrak.h
  Kalimdor/ZulFarrak/zulfarrak.cpp
  Kalimdor/ZulFarrak/instance_zulfarrak.cpp
  Kalimdor/ZulFarrak/boss_zum_rah.cpp
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/boss_epoch_hunter.cpp
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/old_hillsbrad.h
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/boss_leutenant_drake.cpp
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/old_hillsbrad.cpp
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/instance_old_hillsbrad.cpp
  Kalimdor/CavernsOfTime/EscapeFromDurnholdeKeep/boss_captain_skarloc.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/boss_archimonde.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjalAI.h
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjal_trash.h
  Kalimdor/CavernsOfTime/BattleForMountHyjal/boss_kazrogal.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjal_trash.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjal.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjalAI.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/instance_hyjal.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/boss_rage_winterchill.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/hyjal.h
  Kalimdor/CavernsOfTime/BattleForMountHyjal/boss_azgalor.cpp
  Kalimdor/CavernsOfTime/BattleForMountHyjal/boss_anetheron.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/boss_infinite_corruptor.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/boss_salramm_the_fleshcrafter.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/boss_meathook.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/boss_mal_ganis.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/boss_chrono_lord_epoch.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/culling_of_stratholme.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/instance_culling_of_stratholme.cpp
  Kalimdor/CavernsOfTime/CullingOfStratholme/culling_of_stratholme.h
  Kalimdor/CavernsOfTime/TheBlackMorass/the_black_morass.h
  Kalimdor/CavernsOfTime/TheBlackMorass/instance_the_black_morass.cpp
  Kalimdor/CavernsOfTime/TheBlackMorass/boss_chrono_lord_deja.cpp
  Kalimdor/CavernsOfTime/TheBlackMorass/the_black_morass.cpp
  Kalimdor/CavernsOfTime/TheBlackMorass/boss_aeonus.cpp
  Kalimdor/CavernsOfTime/TheBlackMorass/boss_temporus.cpp
  Kalimdor/BlackfathomDeeps/boss_kelris.cpp
  Kalimdor/BlackfathomDeeps/instance_blackfathom_deeps.cpp
  Kalimdor/BlackfathomDeeps/boss_gelihast.cpp
  Kalimdor/BlackfathomDeeps/blackfathom_deeps.cpp
  Kalimdor/BlackfathomDeeps/boss_aku_mai.cpp
  Kalimdor/BlackfathomDeeps/blackfathom_deeps.h
  Kalimdor/Maraudon/boss_princess_theradras.cpp
  Kalimdor/Maraudon/boss_landslide.cpp
  Kalimdor/Maraudon/boss_celebras_the_cursed.cpp
  Kalimdor/Maraudon/boss_noxxion.cpp
  Kalimdor/Maraudon/instance_maraudon.cpp
  Kalimdor/TempleOfAhnQiraj/boss_fankriss.cpp
  Kalimdor/TempleOfAhnQiraj/boss_huhuran.cpp
  Kalimdor/TempleOfAhnQiraj/instance_temple_of_ahnqiraj.cpp
  Kalimdor/TempleOfAhnQiraj/mob_anubisath_sentinel.cpp
  Kalimdor/TempleOfAhnQiraj/boss_viscidus.cpp
  Kalimdor/TempleOfAhnQiraj/boss_twinemperors.cpp
  Kalimdor/TempleOfAhnQiraj/boss_sartura.cpp
  Kalimdor/TempleOfAhnQiraj/boss_cthun.cpp
  Kalimdor/TempleOfAhnQiraj/temple_of_ahnqiraj.h
  Kalimdor/TempleOfAhnQiraj/boss_skeram.cpp
  Kalimdor/TempleOfAhnQiraj/boss_ouro.cpp
  Kalimdor/TempleOfAhnQiraj/boss_bug_trio.cpp
  Kalimdor/RuinsOfAhnQiraj/boss_buru.cpp
  Kalimdor/RuinsOfAhnQiraj/instance_ruins_of_ahnqiraj.cpp
  Kalimdor/RuinsOfAhnQiraj/boss_rajaxx.cpp
  Kalimdor/RuinsOfAhnQiraj/boss_ossirian.cpp
  Kalimdor/RuinsOfAhnQiraj/boss_ayamiss.cpp
  Kalimdor/RuinsOfAhnQiraj/boss_moam.cpp
  Kalimdor/RuinsOfAhnQiraj/ruins_of_ahnqiraj.h
  Kalimdor/RuinsOfAhnQiraj/boss_kurinnaxx.cpp
  Kalimdor/RazorfenKraul/razorfen_kraul.h
  Kalimdor/RazorfenKraul/instance_razorfen_kraul.cpp
  Kalimdor/RazorfenKraul/razorfen_kraul.cpp
  Kalimdor/WailingCaverns/wailing_caverns.h
  Kalimdor/WailingCaverns/instance_wailing_caverns.cpp
  Kalimdor/WailingCaverns/wailing_caverns.cpp
  Kalimdor/OnyxiasLair/boss_onyxia.cpp
  Kalimdor/OnyxiasLair/onyxias_lair.h
  Kalimdor/OnyxiasLair/instance_onyxias_lair.cpp
  Kalimdor/RagefireChasm/instance_ragefire_chasm.cpp
  Kalimdor/DireMaul/instance_dire_maul.cpp
  Kalimdor/HallsOfOrigination/halls_of_origination.h
  Kalimdor/HallsOfOrigination/instance_halls_of_origination.cpp
  Kalimdor/HallsOfOrigination/boss_temple_guardian_anhuur.cpp
  Kalimdor/HallsOfOrigination/boss_earthrager_ptah.cpp
  Kalimdor/HallsOfOrigination/boss_anraphet.cpp
  Kalimdor/Firelands/instance_firelands.cpp
  Kalimdor/Firelands/firelands.h
  Kalimdor/Firelands/boss_alysrazor.cpp
  Kalimdor/WorldBosses/boss_azuregos.cpp
  Kalimdor/Zones/zone_ashenvale.cpp
  Kalimdor/Zones/zone_azshara.cpp
  Kalimdor/Zones/zone_azuremyst_isle.cpp
  Kalimdor/Zones/zone_bloodmyst_isle.cpp
  Kalimdor/Zones/zone_darkshore.cpp
  Kalimdor/Zones/zone_desolace.cpp
  Kalimdor/Zones/zone_durotar.cpp
  Kalimdor/Zones/zone_dustwallow_marsh.cpp
  Kalimdor/Zones/zone_felwood.cpp
  Kalimdor/Zones/zone_feralas.cpp
  Kalimdor/Zones/zone_moonglade.cpp
  Kalimdor/Zones/zone_mulgore.cpp
  Kalimdor/Zones/zone_orgrimmar.cpp
  Kalimdor/Zones/zone_silithus.cpp
  Kalimdor/Zones/zone_stonetalon_mountains.cpp
  Kalimdor/Zones/zone_tanaris.cpp
  Kalimdor/Zones/zone_teldrassil.cpp
  Kalimdor/Zones/zone_the_barrens.cpp
  Kalimdor/Zones/zone_thousand_needles.cpp
  Kalimdor/Zones/zone_thunder_bluff.cpp
  Kalimdor/Zones/zone_ungoro_crater.cpp
  Kalimdor/Zones/zone_winterspring.cpp
)

message("  -> Prepared: Kalimdor")
