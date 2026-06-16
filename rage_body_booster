local g          = ui.create("Lua Rage Booster")
local cb_en      = g:checkbox("Enable Left-Click Baim", false)
local sl_mindmg  = g:slider_int("Left-Click Min Damage", 1, 100, 50) -- Configure the exact override damage threshold

client.set_callback("on_createmove_start", function()
    if not cb_en:get() then return end
    if not cmd.is_valid() then return end

    -- Evaluates if the primary input execution action (Mouse Left Click / Button 1) is active
    if input.is_button_down(1) then
        -- 1. Force Body Aim activation
        -- Commands the internal tracking matrix to prioritize the center mass centroid over precision nodes
        if rage and rage.force_body_aim then
            rage.force_body_aim(true)
        end

        -- 2. Min Damage Override logic
        -- Bypasses general systemic filters to force an instantaneous calculation and discharge cycle
        if rage and rage.set_min_damage then
            rage.set_min_damage(sl_mindmg:get())
        end
    else
        -- Restores the core evaluation logic to default operational profiles once input is released
        if rage and rage.force_body_aim then
            rage.force_body_aim(false)
        end
    end
end)

client.log("rage_body_booster.lua loaded")
