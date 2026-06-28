import streamlit as st

st.set_page_config(page_title="PixelWalls", page_icon="📱", layout="wide")

st.markdown("""
<style>
.main{
    background:#0f172a;
    color:white;
}
.title{
    text-align:center;
    font-size:60px;
    color:#00E5FF;
    font-weight:bold;
}
.sub{
    text-align:center;
    font-size:22px;
    color:white;
}
.box{
    background:#1e293b;
    padding:20px;
    border-radius:15px;
    margin:15px 0;
}
h2{
color:#00E5FF;
}
</style>
""", unsafe_allow_html=True)

# HOME
st.markdown("<div class='title'>📱 PixelWalls</div>", unsafe_allow_html=True)
st.markdown("<div class='sub'>Premium 4K & AMOLED Wallpapers</div>", unsafe_allow_html=True)

st.write("")
st.image("https://images.unsplash.com/photo-1500530855697-b586d89ba3ee", use_container_width=True)

st.write("---")

# PERSONAL DETAILS
st.markdown("<div class='box'>", unsafe_allow_html=True)
st.header("👤 Personal Details")

col1,col2=st.columns([1,2])

with col1:
    st.image("https://cdn-icons-png.flaticon.com/512/3135/3135715.png", width=180)

with col2:
    st.write("### Rajib Pradhan")
    st.write("🎓 CSE (AI & ML) Student")
    st.write("💻 Python Developer")
    st.write("🎨 Wallpaper Designer")
    st.write("📱 Creator of PixelWalls")

st.markdown("</div>", unsafe_allow_html=True)

st.write("---")

# COLLECTION

st.header("🖼️ Wallpaper Collection")

c1,c2,c3=st.columns(3)

with c1:
    st.image("https://picsum.photos/400/700?1")
    st.button("Download AMOLED")

with c2:
    st.image("https://picsum.photos/400/700?2")
    st.button("Download Anime")

with c3:
    st.image("https://picsum.photos/400/700?3")
    st.button("Download Nature")

st.write("---")

# CONTACT

st.header("📩 Contact")

name=st.text_input("Your Name")

email=st.text_input("Email")

msg=st.text_area("Message")

if st.button("Send"):
    st.success("✅ Message Sent Successfully!")

st.write("---")

st.markdown(
"<center>© 2026 PixelWalls | Designed by Rajib Pradhan</center>",
unsafe_allow_html=True
)

