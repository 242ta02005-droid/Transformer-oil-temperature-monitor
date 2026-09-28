# Transformer-oil-temperature-monitor
# Transformer Oil Temperature Monitor

NORMAL_TEMP = 60
WARNING_TEMP = 75
MAX_TEMP = 90

print("==============================")
print(" TRANSFORMER OIL TEMPERATURE MONITOR")
print("==============================")

temperature = float(input("Enter transformer oil temperature (°C): "))

print("\nOil Temperature:", temperature, "°C")

if temperature < 0:
    print("⚠️ Invalid temperature reading")

elif temperature < NORMAL_TEMP:
    print("🟢 OIL TEMPERATURE: NORMAL")
    print("✅ Transformer operating normally")

elif temperature < WARNING_TEMP:
    print("🟡 OIL TEMPERATURE: WARNING")
    print("⚠️ Monitor transformer temperature")

elif temperature < MAX_TEMP:
    print("🟠 OIL TEMPERATURE: HIGH")
    print("🌀 Cooling system should be activated")

else:
    print("🔴 OIL OVERHEATING DETECTED")
    print("⚠️ Protection alert activated")

print("\nTemperature monitoring completed.")
