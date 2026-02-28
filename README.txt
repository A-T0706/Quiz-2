Prompt 1
I accepted the idea that the hero and header shouldn't be resized, but it should change the layout direction. I also accepted the idea to reduce the number of grid coluomns based on the screen width to keep the cards readable on different devices. 
I didn't accept the idea of making a hamburger menu, due to it requiring the use of javascript. 
Prompt 2 
A problem that I encountered was that KPI card would stay to the right on mobile causong horizontal scrolling. They wouldn't align. 
I asked about this:
.hero {
  display: flex;
  padding: 20px;
}

.hero-card {
  width: 240px;
  margin-left: auto;
}
ChatGPT said that a flex container stays in a horizontal row unless you change flex-direction. It said to add a mobile breakpoint to set the hero to a column layout. It also stated that margin-left: auto is useful for pushing the card right on desktop, but on mobile it can create awkward spacing, so it should be reset in the mobile breakpoint.
I added a mobile media query and set the hero layout to stack vertically and I removed the right-align behavior on small screens so the KPI card could sit correctly under the text, with assistance from ChatGPT.
Prompt 3
I tested 375, 768, and 1200
I made sure they met the requirements and had the appropriate amount of columns and that all cards and KPI card are appropriately organized to prevent horizontal scrolling. 
