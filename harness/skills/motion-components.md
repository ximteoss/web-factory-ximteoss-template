# SKILL: ORGANIC MOTION & MICRO-INTERACTIONS

1. **Spring Physics:** Use tactile spring transitions (`transition={{ type: "spring", stiffness: 280, damping: 26 }}`) instead of robotic linear easings.
2. **Scroll-Triggered Reveals:** Wrap major sections in `<motion.div initial={{ opacity: 0, y: 20 }} whileInView={{ opacity: 1, y: 0 }} viewport={{ once: true, margin: "-60px" }}>`.
3. **Tactile Feedback:** Apply subtle lift and press states (`whileHover={{ y: -3 }}` and `whileTap={{ scale: 0.98 }}`) to interactive cards and primary CTAs.