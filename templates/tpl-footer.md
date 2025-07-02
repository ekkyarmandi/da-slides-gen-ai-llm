<style>
  .subtitle {
    color: black;
    opacity: 30%;
    font-weight: 500;
    font-family: 'Fira Code';
    font-size: 16px;
  }
  .uppercase {
    text-transform: uppercase;
  }
 .text-xl {
	 font-size: 1.75rem;
   padding-bottom: 3rem;
 }
 .q {
   font-style: italic;
   font-family: 'Baskerville';
 }
 .text-right {
   text-align: right;
 }
</style>

<grid drag="20 6" drop="topright">
<%? subtitle %>
</grid>

<% content %>

<grid drag="100 6" drop="bottom">
<p class="subtitle">@ekkyarmandi | me@ekky.dev | https://ekky.dev</p>
</grid>

<%? note %>
