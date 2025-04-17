<!DOCTYPE  html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>Conversational PDF Assistant</title><style type="text/css"> * {margin:0; padding:0; text-indent:0; }
 h1 { color: #4BAF4F; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 17.5pt; }
 .p, p { color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; margin:0pt; }
 .h4 { color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 8.5pt; }
 .s1 { color: black; font-family:"Times New Roman", serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 10pt; }
 h2 { color: #2095F2; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 13pt; }
 h3 { color: #FF9800; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 10pt; }
 .s2 { color: #333; font-family:"Times New Roman", serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .s3 { color: #333; font-family:"Courier New", monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .s4 { color: #333; font-family:"Times New Roman", serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .s5 { color: #333; font-family:"Courier New", monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .a, a { color: #0000ED; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: underline; font-size: 8.5pt; }
 .s6 { color: #0000ED; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .s7 { color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 8.5pt; }
 .s8 { color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 .s9 { color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 li {display: block; }
 #l1 {padding-left: 0pt;counter-reset: c1 1; }
 #l1> li>*:first-child:before {counter-increment: c1; content: counter(c1, decimal)". "; color: #FF9800; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 10pt; }
 #l1> li:first-child>*:first-child:before {counter-increment: c1 0;  }
 li {display: block; }
 #l2 {padding-left: 0pt;counter-reset: d1 1; }
 #l2> li>*:first-child:before {counter-increment: d1; content: counter(d1, decimal)". "; color: #FF9800; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 10pt; }
 #l2> li:first-child>*:first-child:before {counter-increment: d1 0;  }
 li {display: block; }
 #l3 {padding-left: 0pt; }
 #l3> li>*:first-child:before {content: "- "; color: #333; font-family:Arial, sans-serif; font-style: normal; font-weight: normal; text-decoration: none; font-size: 8.5pt; }
 li {display: block; }
 #l4 {padding-left: 0pt;counter-reset: d1 4; }
 #l4> li>*:first-child:before {counter-increment: d1; content: counter(d1, decimal)". "; color: #FF9800; font-family:Arial, sans-serif; font-style: normal; font-weight: bold; text-decoration: none; font-size: 10pt; }
 #l4> li:first-child>*:first-child:before {counter-increment: d1 0;  }
 table, tbody {vertical-align: top; overflow: visible; }
</style></head><body><h1 style="padding-top: 3pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Conversational PDF Assistant with RAG (Retrieval-Augmented Generation)</h1><p style="padding-top: 18pt;padding-left: 5pt;text-indent: 0pt;line-height: 145%;text-align: left;">This is an interactive PDF assistant built with <b>Streamlit</b>, designed to help users engage with and extract key information from long PDF documents (including 230+ pages). The app provides a conversational AI interface that offers:</p><p class="s1" style="padding-top: 8pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Document Summarization</span><span class="p">: Automatically generates a concise summary of the uploaded PDF.</span></p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Suggested Questions</span><span class="p">: Displays a list of auto-generated, relevant questions to help users explore the document.</span></p><p class="s1" style="padding-top: 3pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Conversational Q&amp;A</span><span class="p">: Enables users to ask questions about the document&#39;s content with context-aware responses.</span></p><p style="padding-top: 6pt;text-indent: 0pt;text-align: left;"><br/></p><h2 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Features</h2><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><ol id="l1"><li data-list-text="1."><h3 style="padding-left: 17pt;text-indent: -11pt;text-align: left;">PDF Upload and Processing</h3><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><p class="s1" style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="p">Upload large PDF files (including documents with 230+ pages).</span></p><p class="s1" style="padding-top: 3pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAQElEQVQImWPeu3dv0LNnzw4oKSmVzp49+x6js7Pzyw8fPogxMDAwCAoKvmJiQAd79+4NcnFxeeni4vJy7969QQB+rxe9JIBdMQAAAABJRU5ErkJgggAA"/></td></tr></table></span> <span class="p">PDFs are processed, split, and indexed to make them queryable.</span></p><p style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span><span class="p">Generates embeddings using HuggingFace models (</span><span class="s2" style=" background-color: #F4F4F4;"> </span><span class="s3" style=" background-color: #F4F4F4;">all-MiniLM-L6-v2 </span><span class="p">).</span></p><p style="padding-top: 4pt;text-indent: 0pt;text-align: left;"><br/></p></li><li data-list-text="2."><h3 style="padding-left: 16pt;text-indent: -10pt;text-align: left;">Automatic Document Summary</h3><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><p class="s1" style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="p">A brief summary (5–10 key points) is generated from the content of the uploaded PDF to give users an overview of the document.</span></p><p style="padding-top: 4pt;text-indent: 0pt;text-align: left;"><br/></p></li><li data-list-text="3."><h3 style="padding-left: 16pt;text-indent: -10pt;text-align: left;">Auto-Generated Suggested Questions</h3><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span>The app generates <b>5-10 starter questions </b>based on the content of the document, guiding users in their exploration of the material.</p><p style="padding-top: 4pt;text-indent: 0pt;text-align: left;"><br/></p></li><li data-list-text="4."><h3 style="padding-left: 17pt;text-indent: -11pt;text-align: left;">Conversational Q&amp;A (RAG)</h3><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-left: 18pt;text-indent: 0pt;line-height: 145%;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span>Users can engage in a <b>Q&amp;A chat </b>with the assistant, which retrieves relevant context from the document to answer questions. <span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s4"> </span>The assistant responds to queries contextually and remembers the chat history for ongoing sessions.</p><p style="text-indent: 0pt;text-align: left;"><br/></p></li><li data-list-text="5."><h3 style="padding-left: 17pt;text-indent: -11pt;text-align: left;">User-Friendly Interface</h3></li></ol><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><p class="s1" style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Streamlit </span><span class="p">is used to build a clean, intuitive interface.</span></p><p style="padding-top: 3pt;padding-left: 40pt;text-indent: -21pt;line-height: 145%;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span><b>Sections </b>are clearly separated for easy navigation: <span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAQUlEQVQImWPeuXNnKBsb20xDQ8Okjo6OLwxJSUmH//z5w/Tnzx+mpKSkw0wMaIBx586doStXrsxjYGBgCA8PnwQAbnIW8Xrejw8AAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s4"> </span>PDF Upload</p><p class="s1" style="padding-left: 40pt;text-indent: 0pt;line-height: 9pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAQUlEQVQImWPeuXNnKBsb20xDQ8Okjo6OLwxJSUmH//z5w/Tnzx+mpKSkw0wMaIBx586doStXrsxjYGBgCA8PnwQAbnIW8Xrejw8AAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="p">Document Summary</span></p><p style="padding-top: 4pt;padding-left: 40pt;text-indent: 0pt;line-height: 145%;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAQUlEQVQImWPeuXNnKBsb20xDQ8Okjo6OLwxJSUmH//z5w/Tnzx+mpKSkw0wMaIBx586doStXrsxjYGBgCA8PnwQAbnIW8Xrejw8AAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span>Suggested Questions <span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAMklEQVQImWPctm1b1KpVq7IZGBgYwsLCpjIkJCQc+/37N/Pv37+ZExISjjExoAFGdC0AbYYWsf9JmhkAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s4"> </span>Chatbot Interaction</p><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><h2 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Getting Started</h2><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><ol id="l2"><li data-list-text="1."><h3 style="padding-left: 17pt;text-indent: -11pt;text-align: left;">Clone the Repository</h3><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-top: 6pt;padding-left: 5pt;text-indent: 0pt;line-height: 144%;text-align: left;"><span style=" color: #333; font-family:&quot;Courier New&quot;, monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 7pt;">git clone https://github.com/yourusername/conversational-pdf-assistant.git cd conversational-pdf-assistant</span></p><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;"/></li><li data-list-text="2."><h3 style="padding-top: 10pt;padding-left: 17pt;text-indent: -11pt;text-align: left;">Install Required Libraries</h3><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-top: 6pt;padding-left: 5pt;text-indent: 0pt;text-align: left;"><span style=" color: #333; font-family:&quot;Courier New&quot;, monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 7pt;">pip install -r requirements.txt</span></p><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;"/></li><li data-list-text="3."><h3 style="padding-top: 10pt;padding-left: 17pt;text-indent: -11pt;text-align: left;">Set Up Environment Variables</h3><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><div class="textbox" style="background:#F4F4F4;display:block;min-height:15.2pt;width:26.1pt;"><p class="s5" style="padding-top: 2pt;padding-left: 2pt;text-indent: 0pt;text-align: left;">.env</p></div></li></ol><p style="text-indent: 0pt;text-align: left;"/><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Create a    file in the root directory and add the following environment variables:</p><p style="text-indent: 0pt;text-align: left;"><br/></p><p style="padding-top: 6pt;padding-left: 5pt;text-indent: 0pt;line-height: 144%;text-align: left;"><span style=" color: #333; font-family:&quot;Courier New&quot;, monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 7pt;">HF_TOKEN=your_huggingface_api_key GROQ_API_KEY=your_groq_api_key</span></p><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;"/><ul id="l3"><li data-list-text="-"><p style="padding-top: 8pt;padding-left: 11pt;text-indent: -5pt;text-align: left;"><a href="https://huggingface.co/settings/tokens" class="s9" target="_blank">You can get the HuggingFace API key from: </a><a href="https://huggingface.co/settings/tokens" class="a" target="_blank">Hu</a><a href="https://huggingface.co/settings/tokens" class="s6" target="_blank">gg</a><a href="https://huggingface.co/settings/tokens" target="_blank">ing Face</a></p><p style="padding-top: 2pt;text-indent: 0pt;text-align: left;"><br/></p></li><li data-list-text="-"><p style="padding-left: 11pt;text-indent: -5pt;text-align: left;"><a href="https://console.groq.com/" class="s9" target="_blank">You can get the Groq API key from: </a><a href="https://console.groq.com/" target="_blank">Groq Cloud</a></p></li></ul><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><ol id="l4"><li data-list-text="4."><h3 style="padding-left: 17pt;text-indent: -11pt;text-align: left;">Run the Streamlit App</h3></li></ol><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-top: 6pt;padding-left: 5pt;text-indent: 0pt;text-align: left;"><span style=" color: #333; font-family:&quot;Courier New&quot;, monospace; font-style: normal; font-weight: normal; text-decoration: none; font-size: 7pt;">streamlit run app.py</span></p><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;"/><p style="padding-top: 9pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">This will open a new tab in your browser with the interactive app.</p><p style="padding-top: 5pt;text-indent: 0pt;text-align: left;"><br/></p><h2 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">UI Overview</h2><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><h3 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Sections:</h3><p style="padding-top: 4pt;text-indent: 0pt;text-align: left;"><br/></p><p class="s1" style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">PDF Upload Section</span><span class="p">: Upload your PDFs here.</span></p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Summary Section</span><span class="p">: Displays a concise summary of the uploaded document (5-10 key points).</span></p><p class="s1" style="padding-top: 3pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Suggested Questions</span><span class="p">: Provides auto-generated questions based on the document to get you started.</span></p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Q&amp;A Section</span><span class="p">: Interactively ask questions related to the document and receive context-based responses.</span></p><p style="padding-top: 6pt;text-indent: 0pt;text-align: left;"><br/></p><h2 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Tech Stack</h2><p style="padding-top: 3pt;text-indent: 0pt;text-align: left;"><br/></p><table style="border-collapse:collapse;margin-left:7.82296pt" cellspacing="0"><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 28pt;text-indent: 0pt;text-align: left;">Component</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s7" style="padding-top: 7pt;padding-left: 36pt;text-indent: 0pt;text-align: left;">Library/Tool</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">LLM (Language Model)</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Groq API (Gemma2-9b It)</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Embeddings</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">HuggingFace Transformers</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Vector Database</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Chroma</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Text Splitter</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">LangChain RecursiveSplitter</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">UI Framework</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#2B2B2B;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Streamlit</p></td></tr><tr style="height:25pt"><td style="width:108pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#808080;border-right-style:solid;border-right-width:1pt;border-right-color:#2B2B2B"><p class="s7" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Chat History</p></td><td style="width:123pt;border-top-style:solid;border-top-width:1pt;border-top-color:#2B2B2B;border-left-style:solid;border-left-width:1pt;border-left-color:#2B2B2B;border-bottom-style:solid;border-bottom-width:1pt;border-bottom-color:#808080;border-right-style:solid;border-right-width:1pt;border-right-color:#808080"><p class="s8" style="padding-top: 7pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">LangChain ChatHistory</p></td></tr></table><h2 style="padding-top: 12pt;padding-left: 5pt;text-indent: 0pt;text-align: left;">Notes</h2><p style="padding-top: 6pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-left: 18pt;text-indent: 0pt;line-height: 145%;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span>The app works efficiently with <b>large PDFs </b>(including documents over 230 pages). <span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s4"> </span>The document is <b>split into chunks </b>for efficient querying and context retrieval.</p><p style="padding-left: 18pt;text-indent: 0pt;line-height: 9pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span><span class="s1"> </span>The app <b>remembers the chat history </b>across sessions for an enhanced conversational experience.</p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Works best with text-based PDFs</span><span class="p">, not scanned documents (OCR is not included).</span></p><p style="padding-top: 6pt;text-indent: 0pt;text-align: left;"><br/></p><h2 style="padding-left: 5pt;text-indent: 0pt;text-align: left;">Contact</h2><p style="padding-top: 1pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-left: 5pt;text-indent: 0pt;text-align: left;">If you have any questions or need additional features, feel free to reach out!</p><p style="padding-top: 2pt;text-indent: 0pt;text-align: left;"><br/></p><p class="s1" style="padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAPklEQVQImV3BMQHAMAgEwE8rgaU7Wt4AWqoGLx8rHWFCQ/fc3ZKiu7e7v5n5LZI1Mw8AmFlfOEkKkkWyJMUPgHUXxxuEC8EAAAAASUVORK5CYIIA"/></td></tr></table></span> <span class="h4">Developer</span><span class="p">: Sahil Chandel</span></p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAP0lEQVQImV3BMQGAQAwDwD5I6MJeLTFQLa+mWhqsMIapGti5O7s7Jd0RsavqWQA0M5eZmbu/h/2RTAACIJL5AX71F8HaQh1+AAAAAElFTkSuQmCC"/></td></tr></table></span> <span class="h4">Phone Number</span><span class="p">9717891203</span></p><p class="s1" style="padding-top: 4pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAQElEQVQImWPeu3dv0LNnzw4oKSmVzp49+x6js7Pzyw8fPogxMDAwCAoKvmJiQAd79+4NcnFxeeni4vJy7969QQB+rxe9JIBdMQAAAABJRU5ErkJgggAA"/></td></tr></table></span> <span class="h4">Email</span><a href="mailto:sahilchandel.anee@gmail.com" class="s9" target="_blank">: sahilchandel.anee@gmail.com</a></p><p class="s1" style="padding-top: 3pt;padding-left: 18pt;text-indent: 0pt;text-align: left;"><span><table border="0" cellspacing="0" cellpadding="0"><tr><td><img width="4" height="4" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAQAAAAECAYAAACp8Z5+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAAP0lEQVQImV3BMQGAQAwDwD5I6MJeLTFQLa+mWhqsMIapGti5O7s7Jd0RsavqWQA0M5eZmbu/h/2RTAACIJL5AX71F8HaQh1+AAAAAElFTkSuQmCC"/></td></tr></table></span> <span class="h4">GitHub</span><a href="https://github.com/Sahil-Chandel" class="s9" target="_blank">: </a><a href="https://github.com/Sahil-Chandel" target="_blank">Sahil-Chandel GitHub</a></p><p style="padding-top: 3pt;text-indent: 0pt;text-align: left;"><br/></p><p style="padding-left: 5pt;text-indent: 0pt;line-height: 139%;text-align: left;">This app helps you interactively analyze and extract information from PDFs using the latest advancements in AI and document processing. It&#39;s perfect for handling large documents in research, business reports, and any scenario where quick information extraction is key.</p></body></html>
