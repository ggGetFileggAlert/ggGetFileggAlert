-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
username = 'Hello'
SAMPMENU = 1
gg.setVisible(true)
gg.toast("Please wait⏳")
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

function EXIT()
  gg.setVisible(true)
  gg.toast("⛔EXIT⛔")
  gg.clearResults()
  os.exit()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function silent()
  WH1 = gg.choice({
    "🔫🦰SILENT【HEAD】",
    "▶️🚶🏾‍♂️SILENT【BODY】",
    "⁦⁦                            🔙『BACK』🔙",
  }, nil, "🇮🇷[S]amp [C]heats\n 💯creator : @No_Pulse\n 🔰Channel : @Cheaters_Samp")
  if WH1 == 1 then
    hahaha = gg.choice({
        '⌜ ᴏɴ ⌟',
        '⌜ ᴏғғ ⌟',
        ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
      '◤                                                       ◥\n               ◄ silent head ►               \n◣                                                       ◢')

    if hahaha == 1 then silentHead() end
    if hahaha == 2 then silentHeadoff() end
    if hahaha == 3 then silent() end
  end
  if WH1 == 2 then
    hah = gg.choice({
        '⌜ ᴏɴ ⌟',
        '⌜ ᴏғғ ⌟',
        ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
      '◤                                                       ◥\n               ◄ silent body ►               \n◣                                                       ◢')

    if hah == 1 then silentBody() end
    if hah == 2 then silentBodyoff() end
    if hah == 3 then silent() end
  end

  if WH1 == 3 then HOME() end
  SAMPMENU = -1
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-- on head
function silentHead()
  gg.processResume()
  gg.searchNumber("1,042,536,202", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.processResume()
  gg.getResults(400, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.processResume()
  gg.editAll("1,070,300,300", gg.TYPE_DWORD)
  gg.toast('[' .. username .. ']' .. " Cheat Active✅")
  gg.clearResults()
  silent()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

-- on body
function silentBody()
  data2 = 0
  gg.setVisible(false)
  settings2 = gg.prompt({
      "type range: [1;55]" },
    { nil },
    { 'number' })

  number2 = tonumber(settings2[1])
  range2 = 45 + number2
  gg.processResume()
  gg.searchNumber("1,043,878,380", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.processResume()
  gg.getResults(400, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.processResume()
  gg.editAll("1,0" .. tostring(range2) .. ",350,350", gg.TYPE_DWORD)
  gg.toast('[' .. username .. ']' .. " Cheat Active✅")
  gg.clearResults()
  silent()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


-- off head
function silentHeadoff()
  gg.processResume()
  gg.searchNumber("1,070,300,300", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.processResume()
  gg.getResults(400, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.processResume()
  gg.editAll("1,042,536,202", gg.TYPE_DWORD)
  gg.toast('[' .. username .. ']' .. " Cheat Deactive✅")
  gg.clearResults()
  silent()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-- off body

function silentBodyoff()
  gg.processResume()
  gg.searchNumber("1,0" .. tostring(range2) .. ",350,350", gg.TYPE_DWORD, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.processResume()
  gg.getResults(400, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.processResume()
  gg.editAll("1,043,878,380", gg.TYPE_DWORD)
  gg.toast('[' .. username .. ']' .. " Cheat Deactive✅")
  gg.clearResults()
  silent()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-- tpALPHA
function tpALPHA()
gg.setRanges(gg.REGION_C_ALLOC)
 gg.searchNumber("0.0;1.0;0.0;1,376.5;67.0859375;0.0;0.0;0.0::33", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1) 
  if gg.getResultCount() == 19 then
  gg.alert("TELEPORT faild")
  else
  gg.setVisible(false)
  gg.refineNumber("1,376.5", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
n = gg.getResultCount()
ms = gg.getResults(n)
for CHEATERS_SAMP = 1, n do
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 84, flags = 16, freeze = true, value = 2046.3 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 80, flags = 16, freeze = true, value = -1913.2 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 252, flags = 16, freeze = true, value = 12 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 248, flags = 16, freeze = true, value = 2046.3 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 244, flags = 16, freeze = true, value = -1913.2 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 76, flags = 16, freeze = true, value = 12 } })
  gg.sleep(800)
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 84, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 80, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 252, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 248, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 244, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 76, flags = 16, freeze = false, value = 0 } })
    gg.clearResults()
  gg.loadResults(gg.getListItems())
local t = gg.getResults(3)
gg.removeResults(t)
 gg.removeListItems(gg.getListItems())

 tpStart()



end
end
end

function tpStart()
	gg.sleep(400)
	job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400) 
	job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(600)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("2046.3;-1913.2;12", gg.TYPE_FLOAT)
	gg.sleep(400)
    gg.toast('Cheat Activated✅')
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
-- tpFLIN
function tpFLIN()
gg.setRanges(gg.REGION_C_ALLOC)
 gg.searchNumber("0.0;1.0;0.0;1,376.5;67.0859375;0.0;0.0;0.0::33", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1) 
  if gg.getResultCount() == 19 then
  gg.alert("TELEPORT faild")
  else
  gg.setVisible(false)
  gg.refineNumber("1,376.5", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
n = gg.getResultCount()
ms = gg.getResults(n)
for CHEATERS_SAMP = 1, n do
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 84, flags = 16, freeze = true, value = 1419.16 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 80, flags = 16, freeze = true, value = -1623.57 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 252, flags = 16, freeze = true, value = 13.54 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 248, flags = 16, freeze = true, value = 2046.3 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 244, flags = 16, freeze = true, value = -1913.2 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 76, flags = 16, freeze = true, value = 12 } })
  gg.sleep(800)
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 84, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 80, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 252, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 248, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 244, flags = 16, freeze = false, value = 0 } })
  gg.addListItems({ [1] = { address = ms[CHEATERS_SAMP].address - 76, flags = 16, freeze = false, value = 0 } })
    gg.clearResults()
  gg.loadResults(gg.getListItems())
local t = gg.getResults(3)
gg.removeResults(t)
 gg.removeListItems(gg.getListItems())

 tpStart()



end
end
end

function tpStart()
	gg.sleep(400)
	job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(400) 
	job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(500)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(400)
    job = gg.getResults(50, nil, nil, nil, nil, nil, nil, nil, nil)
	gg.editAll("1419.16;-1623.57;13.54", gg.TYPE_FLOAT)
	gg.sleep(400)
    gg.toast('Cheat Activated✅')
end


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function tpselector()
  tpselec = gg.alert("Which one ?", "🔵AlphaRp🔵", "🟡FlinRP🟡", "🔁BACK🔁")
  if tpselec == nil then tpselector() end
  if tpselec == 1 then tpALPHA() end
  if tpselec == 2 then tpFLIN() end
  if tpselec == 3 then HOME() end
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function gunwar()
  gg.setRanges(gg.REGION_C_ALLOC)
  gg.clearResults()
  gg.searchNumber("1.40129846e-45;0.0;0.0;0.0;0.0;7.5::41", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
  gg.setVisible(false)
  if gg.getResultCount(1) == 0 then
    gg.alert("healt hack faild⛔⛔")
  else
    gg.searchNumber("1.40129846e-45", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
    n = gg.getResultCount()
    ms = gg.getResults(n)
    for EVIL = 1, n do
      gg.addListItems({ [1] = { address = ms[EVIL].address + 8, flags = 16, freeze = true, value = 101 } })
      --  gg.addListItems({ [1] = { address = ms[EVIL].address + 16, flags = 16, freeze = false, value = 100 } })
      gg.setRanges(gg.REGION_C_ALLOC)
      gg.clearResults()
      gg.searchNumber("101.0;7.5::33", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
      gg.setVisible(false)
      if gg.getResultCount() == 0 then
      else
        gg.searchNumber("7.5", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
        n = gg.getResultCount()
        ms = gg.getResults(n)
        for EVIL = 1, n do
          gg.addListItems({ [1] = { address = ms[EVIL].address + 92, flags = 4, freeze = true, value = 8 } })

          gg.addListItems({ [1] = { address = ms[EVIL].address + 120, flags = 4, freeze = true, value = 24 } })
          gg.addListItems({ [1] = { address = ms[EVIL].address + 128, flags = 4, freeze = true, value = 7 } })
          gg.addListItems({ [1] = { address = ms[EVIL].address + 132, flags = 4, freeze = true, value = 12000 } })

          gg.addListItems({ [1] = { address = ms[EVIL].address + 204, flags = 4, freeze = true, value = 30 } })
          gg.addListItems({ [1] = { address = ms[EVIL].address + 212, flags = 4, freeze = true, value = 30 } })
          gg.addListItems({ [1] = { address = ms[EVIL].address + 216, flags = 4, freeze = true, value = 12000 } })

          gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
        end
      end
    end
  end
end

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function speedfire()
  spd = gg.choice({
      '⌜ ᴏɴ ⌟',
      '⌜ ᴏғғ ⌟',
      ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
    '◤                                                       ◥\n               ◄ SpeedFire ►               \n◣                                                       ◢')

  if spd == 1 then
    gg.toast('[' .. username .. ']' .. ' Loading...')
    gg.sleep(200)
    gg.setSpeed(1.2)
    gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  end
  if spd == 2 then
    gg.toast('[' .. username .. ']' .. ' Loading...')
    gg.sleep(200)
    gg.setSpeed(1.0)
    gg.toast('[' .. username .. ']' .. ' Cheat Deactive ✅')
  end
  if spd == 3 then HOME() end
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function slow()
  slw = gg.choice({
      '⌜ ᴏɴ ⌟',
      '⌜ ᴏғғ ⌟',
      ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
    '◤                                                       ◥\n               ◄ Slow Motion ►               \n◣                                                       ◢')

  if slw == 1 then
    gg.toast('[' .. username .. ']' .. ' Loading...')
    gg.sleep(200)
    gg.setSpeed(0.8)
    gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  end
  if slw == 2 then
    gg.toast('[' .. username .. ']' .. ' Loading...')
    gg.sleep(200)
    gg.setSpeed(1.0)
    gg.toast('[' .. username .. ']' .. ' Cheat Deactive ✅')
  end
  if slw == 3 then HOME() end
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function fpsup()
  gg.sleep(300)
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function speedspr()
  sps = gg.choice({
      '⌜ ᴏɴ ⌟',
      '⌜ ᴏғғ ⌟',
      ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
    '◤                                                       ◥\n               ◄ sᴘᴇᴇᴅ sᴘʀɪɴᴛ ►               \n◣                                                       ◢')

  if sps == 1 then dv1() end
  if sps == 2 then dv2() end
  if sps == 3 then HOME() end
end

function dv1()
  gg.setRanges(gg.REGION_C_DATA)
  gg.searchNumber("4.0;0.69999998808;0.20000000298;5.0;10.0;1.0;0.5;0.30000001192:29", gg.TYPE_FLOAT, false,
    gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("0.7", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll('-0.565651', gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  gg.clearResults()
end

function dv2()
  gg.setRanges(gg.REGION_C_DATA)
  gg.searchNumber("4.0;-0.565651;0.20000000298;5.0;10.0;1.0;0.5;0.30000001192:29", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0,
    -1, 0)
  gg.refineNumber("-0.565651", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll('0.7', gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Deactive ✅')
  gg.clearResults()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function wallhack()
  gg.setRanges(gg.REGION_CODE_APP)
  gg.searchNumber("60", gg.TYPE_FLOAT)
  gg.getResults(10)
  gg.editAll("18.9", gg.TYPE_FLOAT)
  gg.clearResults()
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  gg.clearResults()
  gg.setVisible(false)
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function gmcar()
  gg.searchNumber(1000, gg.TYPE_FLOAT)
  gg.getResults(84)
  gg.editAll(1000000000, gg.TYPE_FLOAT)
  gg.clearResults()
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function slap()
  gg.setRanges(gg.REGION_C_DATA | gg.REGION_CODE_APP)
  gg.searchNumber("0.00000911894;-0.08607242256;0.00800000038;-0.00800000038:13", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0,
    -1, 0)
  gg.refineNumber("0.008", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(5000, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll("-1", gg.TYPE_FLOAT)
  gg.editAll("0.0008", gg.TYPE_FLOAT)
  gg.sleep(2000)
  gg.editAll("0.009", gg.TYPE_FLOAT)
  gg.sleep(500)
  gg.editAll("0.0008", gg.TYPE_FLOAT)
  gg.sleep(1000)
  gg.editAll("0.008", gg.TYPE_FLOAT)
  gg.sleep(500)
  gg.editAll("0.0008", gg.TYPE_FLOAT)
  gg.sleep(1000)
  gg.editAll("0.008", gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  gg.clearResults()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function fh()
  fas = gg.choice({
      '⌜ ᴏɴ ⌟',
      '⌜ ᴏғғ ⌟',
      ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
    '◤                                                       ◥\n               ◄ ғᴀsᴛ fist ►               \n◣                                                       ◢')

  if fas == 1 then fh1() end
  if fas == 2 then fh2() end
  if fas == 3 then HOME() end
end

function fh1()
  gg.setRanges(gg.REGION_C_DATA | gg.REGION_CODE_APP)
  gg.searchNumber(
    "0.20000000298F;0.69999998808F;-0.20000000298F;-0.10000000149F;0.80000001192F;3000.0F;150.0F;2000.0F;176.0F",
    gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("-0.2", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(999, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll("-2", gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  gg.clearResults()
end

function fh2()
  gg.setRanges(gg.REGION_C_DATA)
  gg.searchNumber("0.20000000298F;0.69999998808F;-2F;-0.10000000149F;0.80000001192F;3000.0F;150.0F;2000.0F;176.0F",
    gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("-2", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll('-0.2', gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Deactive ✅')
  gg.clearResults()
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function ipadView()
  gg.setRanges(gg.REGION_CODE_APP)
  gg.searchNumber("360.0;0.00100000005;-9.38575022e22", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
  gg.refineNumber("360.0", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1)
  gg.getResults(2)
  gg.editAll("254.70928955078", gg.TYPE_FLOAT)
  gg.clearResults()

  gg.clearResults()

  gg.searchNumber("3.60", gg.TYPE_FLOAT)

  gg.toast("50%")
  gg.getResults(1000)

  gg.editAll("-2.60", gg.TYPE_FLOAT)

  gg.clearResults()

  gg.searchNumber("70", gg.TYPE_FLOAT)

  gg.getResults(1000)

  gg.editAll("120",
    gg.TYPE_FLOAT)

  gg.clearResults()

  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
function gm()
  gg.setRanges(gg.REGION_C_ALLOC)
  gg.searchNumber("8~100;100.06400146484~150.66400146484;7.5:33", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("8~101", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(999, nil, nil, nil, nil, nil, nil, nil, nil)
  revert = gg.getResults(999, nil, nil, nil, nil, nil, nil, nil, nil)
  local t = gg.getResults(999, nil, nil, nil, nil, nil, nil, nil, nil)
  for i, v in ipairs(t) do
    if v.flags == gg.TYPE_FLOAT then
      v.value = "500000000000.0"
      v.freeze = true
    end
  end
  gg.addListItems(t)
  t = nil
  gg.clearResults()
  gg.toast(' ╔ ᴀᴄᴛɪᴠᴀᴛᴇᴅ ╗ ')
end

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

function hj()
  khhhhhhhhhhhh = gg.choice({
      '⌜ ᴏɴ ⌟',
      '⌜ ᴏғғ ⌟',
      ' ⟪ ʙᴀᴄᴋ ⟫ ' }, nil,
    '◤                                                       ◥\n               ◄ ʜɪɢʜᴊᴜᴍᴘ ►               \n◣                                                       ◢')

  if khhhhhhhhhhhh == 1 then hj1() end
  if khhhhhhhhhhhh == 2 then hj2() end
  if khhhhhhhhhhhh == 3 then HOME() end
end

function hj1()
  gg.setRanges(gg.REGION_C_DATA | gg.REGION_CODE_APP)
  gg.searchNumber("0.69999998808;-0.20000000298;-0.10000000149:17", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("-0.1", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(999, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll("-60", gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Active ✅')
  gg.clearResults()
end

function hj2()
  gg.setRanges(gg.REGION_C_DATA)
  gg.searchNumber("0.69999998808;-0.20000000298;-60:17", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  gg.refineNumber("-60", gg.TYPE_FLOAT, false, gg.SIGN_EQUAL, 0, -1, 0)
  revert = gg.getResults(100000, nil, nil, nil, nil, nil, nil, nil, nil)
  gg.editAll('-0.1', gg.TYPE_FLOAT)
  gg.toast('[' .. username .. ']' .. ' Cheat Deative ✅')
  gg.clearResults()
end


function HOME()
  MultiMenu = gg.choice(
    { "💥Silent Aim💥", "🏙TP To DmZone🏙", "🔫GUN FOR WAR🔫", "🎭CBUG Zed Rec🎭", "🎃Slow Motion🎃",
      "👓Fast Run👓", "💎FPS BOOST💎", "📱Wall Hack📱", "🚑GM Car🚑", "🚀Slap🚀", "👊Fast Fist👊",
      "👀Ipad View(360)👀", "♥God Mode♥", "👟High Jump👟", "🚫EXIT" }, nil,
    "============================\n🗣UserName: " ..
    username ..
    "\n============================\n⏳now : " ..
    os.date("%Y") ..
    "/" ..
    os.date("%m") ..
    "/" ..
    os.date("%d") ..
    "\n⏳Expired in : 2025/1/5" ..
    "\n💎Creator : [PKN] @No_Pulse\n🌎Channel : @Cheaters_Samp")
  if MultiMenu == nil then
    SAMPMENU = -1
  else
    if MultiMenu == 1 then silent() end
    if MultiMenu == 2 then tpselector() end
    if MultiMenu == 3 then gunwar() end
    if MultiMenu == 4 then speedfire() end
    if MultiMenu == 5 then slow() end
    if MultiMenu == 6 then speedspr() end
    if MultiMenu == 7 then fpsup() end
    if MultiMenu == 8 then wallhack() end
    if MultiMenu == 9 then gmcar() end
    if MultiMenu == 10 then slap() end
    if MultiMenu == 11 then fh() end
    if MultiMenu == 12 then ipadView() end
    if MultiMenu == 13 then gm() end
    if MultiMenu == 14 then hj() end
    if MultiMenu == 15 then EXIT() end
  end
  SAMPMENU = -1
end

while (true) do
  if gg.isVisible(true) then
     SAMPMENU = 1
     gg.setVisible(false)
     HOME()
 end
end

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- 
