# Calculadora ADA — SimpliRoute

Calculadora dinámica para cotizar paquetes combinados de **Llamadas + WhatsApp + SimpliChat** con margen, markup estructural y descuento comercial.

## Uso
Abrí `index.html` en cualquier browser moderno. Es 100% client-side, no necesita backend.

## Fórmulas
```
costo_variable = cantidad × costo_unitario
subtotal_variable = Σ costo_variable
markup_estructural = subtotal_variable × (% / 100)
costo_interno = subtotal_variable + markup_estructural
precio = costo_interno / (1 - margen)
precio_final = precio × (1 - descuento)
```

## Costos (defaults)
- Llamadas: $0.50/min (peor caso — Twilio + ElevenLabs + Gemini)
- WhatsApp: $0.25/conversación (Meta + Kaps + Gemini + Maps)
- SimpliChat: $0.15/conversación (Stream + Gemini)

## Demo
https://gigioagente-jpg.github.io/calculadora-ada/
